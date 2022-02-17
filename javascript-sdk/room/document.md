# Room SDK

二人以上の複数人でのメディア通信を行うアプリケーションを簡単に作るための SDK です。
通信方式を P2P と SFU の 2 種類から選択可能です。

# インストール方法

```sh
npm i @skyway-nv/room
```

# 概要

アプリケーションのクライアントはメディア通信を開始するまでに次のようなフローをたどります。

**1. Token を入手する**

SkyWay サービスはユーザの認証認可に独自の JWT Token を使用しています。
この Token は 2 種類の方法で入手することができます。

- アプリケーションサーバサイドで生成したトークンをクライアントで使用する
- クライアント上でトークンを生成して使用する

後者の方法だと正しく権限の制限をすることができないので前者の方法を取ることを推奨します。

**2. Room を作成する**

メディア通信を行うグループの単位を Room と呼びます。
メディア通信を開始するにはまず Room を作る権限を持った Token を用いて Room を作成する必要があります。

**3. クライアントが Room に Join して Room の Member となる**

この際に Room に参加する権限を持った Token とともに Room に Join する必要があります

**4. メディアの Stream を Room 内に Publish および Subscribe する**

Member が Stream を Publish すると Room 上に Stream の情報である Publication というリソースが生成されます。

他の Member はこの Publication を Subscribe すると Subscription というリソースが Room 上に生成され、Subscription に対応する Stream を受信し、メディア通信が開始できます。

# 用語解説

Room SDK の用語、仕様について説明します。

## Room

複数の Member が通信するグループの単位です。

それぞれの Member は Room 内にいる他の Member と映像/音声/データの送受信が出来ます。

通信方式を P2P と SFU の 2 種類から選択可能です。

### Room ID

Room ID は SkyWay サービスによって設定される Room を一意に識別するための ID です。

### Room Name

Room Name はユーザが Room を作成する際に指定することができる任意の値です。

アプリケーション内で重複した Room Name を指定することはできません。

## Member

Member は他のクライアントとの通信を管理するエージェントです。

映像や音声を送信したり、受信したりすることが出来ます。

### Member ID

Member ID は SkyWay サービスによって設定される Member を一意に識別するための ID です。

### Member Name

Member Name はクライアントが Room に Join する際に指定することができる任意の値です。

Room 内で重複した Member Name を指定することはできません。

## Stream

Room 内で Member が通信するメディアのことを Stream と呼びます。

三種類の Stream が存在します。

- VideoStream
- AudioStream
- DataStream

## Publication

あるクライアントが用意した Stream を他の Member が受信可能にするために Room 内に公開する操作のことを Publish と呼びます。Stream を Publish すると Room 内に Publication というリソースが生成されます。

他の Member は Publication を Subscribe することで Subscription というリソースを得られて、Stream の受信が開始されます。

Publication を Unpublish すると SkyWay サービス側で関連する Subscription を Unsubscribe して削除します。

## Subscription

あるクライアントが Room に存在する Publication を Subscribe した時に得られるリソースです。Subscription には Stream が含まれており、メディアの受信が可能です。

Room 内の Subscription を見ることでどの Member がどの Publication を Subscribe しているかを把握することができます。

クライアントの Member が Subscribe していない Subscription の Stream を参照することはできません。Member が Stream を受信するためには必ずその Member が Publication を Subscribe して Subscription を作る必要があります。

Subscription と紐ついている Publication が Unpublish されると Subscription は自動的に Unsubscribe されます。

# クラス一覧

- SkyWayContext
- Room
  - P2PRoom
  - SfuRoom
- Member
  - LocalRoomMember
  - RemoteRoomMember
- SkyWayMediaDevices
- RoomPublication
- RoomSubscription

## SkyWayContext

アプリケーションの設定を行います。

```ts
import { SkyWayContext } from '@skyway-nv/room';

const context = await SkyWayContext.Create(tokenString);
```

事前にトークンの取得が必要になります。

### トークンの取得方法

SkyWay サービスの JWT トークンはトークンの仕様に基づいて自身で作成するか、`@skyway-nv/token`ライブラリを使って作成することができます。

`@skyway-nv/token`ライブラリは Node.js サーバとブラウザで動作しますが、トークンでユーザの行動を認可したい場合は必ずサーバ側でトークンを作成して下さい。

```ts
import { SkyWayAuthToken } from '@skyway-nv/token';

const token = new SkyWayAuthToken(parameters);
const tokenString = token.encode('secret');
```

## Room

Member の参加する Room の作成/取得を行います。

**作成**

新しい Room を作成します。

```ts
import { SkyWayContext, SkyWayRoom } from '@skyway-nv/room';

const context = await SkyWayContext.Create(tokenString);
const room = await SkyWayRoom.Create(context, {
  type: 'p2p',
  id: 'something',
});
```

Room 作成時に、RoomType を指定する必要があります。

- type
  - `p2p` もしくは `sfu`

Room 作成時に、任意の RoomId を指定することができます。

**取得**

既存の Room を取得します。

```ts
import { SkyWayContext, SkyWayRoom } from '@skyway-nv/room';

const context = await SkyWayContext.Create(tokenString);
const room = await SkyWayRoom.Find(context, roomId, roomType);
```

**取得もしくは作成**

任意の Room の取得を試みて、存在しなければ作成します。

```ts
import { SkyWayContext, SkyWayRoom } from '@skyway-nv/room';

const context = await SkyWayContext.Create(tokenString);
const room = await SkyWayRoom.FindOrCreate(context, {
  type: 'sfu',
  id: 'channelId',
});
```

## P2PRoom / SfuRoom

Room には P2PRoom と SfuRoom の 2 種類が存在します。
API は P2PRoom と SfuRoom で共通しています。

### Member の Room への参加

```ts
const member: LocalRoomMember = await room.join();
```

Room に参加すると LocalRoomMember インスタンスを取得できます。

### Room の情報にアクセスする

**Member**

Stream の Member の情報のリストを参照することが出来ます。

```ts
const members = room.members;
```

**Publication**

Stream の Publication のリストを参照することが出来ます。

```ts
const publications = room.publications;
```

**Subscription**

Stream の Subscription のリストを参照することが出来ます。

```ts
const subscriptions = room.subscriptions;
```

## LocalRoomMember

Stream の Publish、Subscribe などを行うことが出来ます。

### Stream の Publish

Room に Stream を Publish することができます。

```ts
import { SkyWayMediaDevices } from '@skyway-nv/room';

...

const video = await SkyWayMediaDevices.createCameraVideoStream();
const publication = await member.publish(video,options);
```

Room の種類によって Publish 時に指定できる Option が異なります。

**P2P**

```ts
interface Option {
  metadata?: string | undefined;
  codecCapabilities?: Codec[];
  encodings?: EncodingParameters[];
}
```

**SFU**

```ts
interface Option {
  metadata?: string | undefined;
  codecCapabilities?: Codec[];
  encodings?: EncodingParameters[];
  maxSubscribers?: number;
}
```

maxSubscribers では Publish した Stream を Subscribe できる数の上限値を指定できます。指定しない場合、maxSubscribers には 10 がセットされます。

Simulcast を利用する場合は encodings に複数のパラメータをセットします

```ts
const video = await SkyWayMediaDevices.createCameraVideoStream();
const publication = await member.publish(video, {
  encodings: [
    // 複数のパラメータをセットする
    { maxBitrate: 10_000, scaleResolutionDownBy: 8 },
    { maxBitrate: 680_000, scaleResolutionDownBy: 1 },
  ],
});
```

### Stream の Unpublish

Room 上の Stream の Publication を Unpublish することができます。
関連する Subscription が自動的に Unsubscribe されます。

```ts
await member.unpublish(publication.id);
```

### Stream の Subscribe

Room 上の Stream の Publication を Subscribe することができます。

```ts
const { subscription, stream } = await member.subscribe(publication.id);
```

### Stream の Unsubscribe

Subscribe している Stream の Subscription を Unsubscribe することができます。

```ts
await member.unsubscribe(subscription.id);
```

### Metadata の更新

Member に紐付いた Metadata を更新することができます

```ts
await member.updateMetadata('metadata');
```

## SkyWayMediaDevices

各種 Stream の取得が出来ます。

**マイク**

```ts
const audio = await SkyWayMediaDevices.createMicrophoneAudioStream(options);
```

**カメラ**

```ts
const video = await SkyWayMediaDevices.createCameraVideoStream(options);
```

**DataChannel**

※SFU Room では使用できません。

```ts
const data = await SkyWayMediaDevices.createDataStream();
```

### AudioStream / VideoStream の利用方法

SkyWay の Stream を Html で再生する方法が 2 種類あります。

**element に適用する**

HtmlAudioElement / HtmlVideoElement に Stream を適用することが出来ます。

```ts
const localVideo = document.getElementById(
  'js-local-stream'
) as HTMLVideoElement;
localVideo.muted = true;
localVideo.playsInline = true;

// 適用する
skywayStream.attach(localVideo);

await localVideo.play();
```

**MediaStream を作る**

MediaStream を作成して使うことが出来ます。

```ts
const stream = new MediaStream([
  // MediaStreamTrackにアクセスできる
  skywayStream.track,
]);
```

## RoomPublication

Publication の情報の参照と Publication の操作ができます

### Metadata の更新

Publication に紐付いた Metadata を更新することができます

```ts
await publication.updateMetadata('metadata');
```

## RoomSubscription

Subscription の情報の参照と Subscription の操作ができます

### Stream の参照

Subscription から映像/音声/データの Stream を参照できます。
ローカルで Subscribe している Subscription でなければ undefined となります

```ts
const stream = subscription.stream;
if (stream.contentType === 'data') {
  stream.onData.add((data) => {
    console.log(data);
  });
} else {
  const track = stream.track;
}
```
