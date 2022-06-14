@skyway-sdk/room / [Exports](modules.md)

# Room

複数人で通信をするアプリケーションを作るための ライブラリ です。
通信方式を P2P と SFU の 2 種類から選択できます。

# インストール方法

```sh
npm i @skyway-sdk/room
```

# 概要

クライアントアプリケーションは通信を開始するまでに以下のフローをたどります。

**1. SkyWay Auth Token を取得（生成）する**

[SkyWay Auth Token について](https://beta.skyway.ntt.com/auth-token.html)

**2. Room を作成する**

メディア通信を行うグループの単位を Room と呼びます。
メディア通信を開始するにはまず Room を作る権限を持った SkyWay Auth Token を用いて Room を作成する必要があります。

**3. クライアントが Room に Join して Room の Member となる**

**4. Stream を Room 内に Publish および Subscribe する**

Member が Stream を Publish すると Room 上に Stream の情報である Publication というリソースが生成されます。

他の Member はこの Publication を Subscribe すると Subscription というリソースが Room 上に生成され、Subscription に対応する Stream を受信し、通信を開始できます。

# 用語解説

Room ライブラリ の用語、仕様について説明します。

## Room

複数の Member が通信するグループの単位です。

それぞれの Member は Room 内にいる他の Member と映像/音声/データの送受信が出来ます。（なお、SFU Room の場合はデータの送受信ができません。）

通信方式を P2P と SFU の 2 種類から選択可能です。

Room は 一意な識別子である ID と、オプショナルな値である Name を持ちます。

ID は Room 作成時に自動的に払い出される値であり、Name はユーザが Channel を作成する際に指定することができる任意の値です。

また、アプリケーション内で重複した Name を指定することはできません。

## Member

Member は他のクライアントとの通信を管理するエージェントです。

映像や音声を送信したり、受信したりすることが出来ます。

Member は 一意な識別子である ID と、オプショナルな値である Name を持ちます。

ID は Member 作成時に自動的に払い出される値であり、Name はクライアントが Channel に Join する際に指定することができる任意の値です。

Room 内で重複した Name を指定することはできません。

## Stream

Room 内で Member が通信する映像/音声/データを Stream と呼びます。

三種類の Stream が存在します。

- VideoStream
- AudioStream
- DataStream

## Publication

あるクライアントが用意した Stream を他の Member が受信可能にするために Room 内に公開する操作のことを Publish と呼びます。Stream を Publish すると Room 内に Publication というリソースが生成されます。

他の Member は Publication を Subscribe することで Subscription というリソースを得られて、Stream の受信が開始されます。

Publication を Unpublish すると SkyWay サービス側で関連する Subscription を Unsubscribe して削除します。

## Subscription

あるクライアントが Room に存在する Publication を Subscribe した時に得られるリソースです。Subscription には Stream が含まれており、映像・音声・データの受信が可能です。

Room 内の Subscription のプロパティを確認することで、どの Member がどの Publication を Subscribe しているかを把握することができます。

クライアントの Member が Subscribe していない Subscription の Stream を参照することはできません。Member が Stream を受信するためには必ずその Member が Publication を Subscribe して Subscription を作る必要があります。

Subscription と紐ついている Publication が Unpublish されると Subscription は自動的に Unsubscribe されます。

# 基本機能

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
import { SkyWayContext } from '@skyway-sdk/room';

const context = await SkyWayContext.Create(tokenString);
```

事前に SkyWay Auth Token の取得が必要になります。

### SkyWay Auth Token の取得方法

SkyWay Auth Token は、仕様に基づいて自身で作成するか、`@skyway-sdk/token`ライブラリを使って作成することができます。

`@skyway-sdk/token`ライブラリは Node.js サーバとブラウザで動作しますが、SkyWay Auth Token でユーザの行動を認可したい場合は必ずサーバ側で作成して下さい。

```ts
import { SkyWayAuthToken } from '@skyway-sdk/token';

const token = new SkyWayAuthToken(parameters);
const tokenString = token.encode('secret');
```

## Room

Member の参加する Room の作成/取得を行います。

### 作成

新しい Room を作成します。

```ts
import { SkyWayContext, SkyWayRoom } from '@skyway-sdk/room';

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

### 取得

既存の Room を取得します。

```ts
import { SkyWayContext, SkyWayRoom } from '@skyway-sdk/room';

const context = await SkyWayContext.Create(tokenString);
const room = await SkyWayRoom.Find(context, roomId, roomType);
```

### 取得もしくは作成

任意の Room の取得を試みて、存在しなければ作成します。

```ts
import { SkyWayContext, SkyWayRoom } from '@skyway-sdk/room';

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
const member: LocalRoomMember = await room.join({
  name: 'something',
  metadata: 'something',
});
```

Room に参加すると LocalRoomMember インスタンスを取得できます。

追加時に`name`と`metadata`の設定が可能です。(optional)

`name`は Room 内の他の Member と重複することはできません。

join を複数回実行して に複数の LocalRoomMember を取得することはできません。

### Room の情報にアクセスする

#### Member

Stream の Member の情報のリストを参照することが出来ます。

```ts
const members = room.members;
```

#### Publication

Stream の Publication のリストを参照することが出来ます。

```ts
const publications = room.publications;
```

#### Subscription

Stream の Subscription のリストを参照することが出来ます。

```ts
const subscriptions = room.subscriptions;
```

## LocalRoomMember

Stream の Publish、Subscribe などを行うことが出来ます。

### Stream の Publish

Room に Stream を Publish することができます。

```ts
import { SkyWayMediaDevices } from '@skyway-sdk/room';

...

const video = await SkyWayMediaDevices.createCameraVideoStream();
const publication = await member.publish(video,options);
```

Room の種類によって Publish 時に指定できる Option が異なります。

#### P2P

```ts
interface Option {
  metadata?: string | undefined;
  codecCapabilities?: Codec[];
  encodings?: EncodingParameters[];
}
```

#### SFU

```ts
interface Option {
  metadata?: string | undefined;
  codecCapabilities?: Codec[];
  encodings?: EncodingParameters[];
  maxSubscribers?: number;
}
```

maxSubscribers では Publish した Stream を Subscribe できる数の上限値を指定できます。指定しない場合、maxSubscribers には 10 がセットされます。

なお、SkyWay Beta 提供中は以下の制限があります。制限値は 50 人での双方向通信を想定した値に基づいております。

- maxSubscribers の最大値: 49
- アプリケーションにおける、AudioPublication の maxSubscribers の合計値: 2450 (49 人 x 50 人)
- アプリケーションにおける、VideoPublication の maxSubscribers の合計値: 2450 (49 人 x 50 人)

##### Simulcast 機能の利用方法

VideoStream を Publish する際に複数のエンコード設定を指定することで、受信側クライアントデバイスが通信品質に合わせて自動的に最適なエンコード設定の映像を受け取る機能を利用できます。

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

#### コーデックの指定方法

メディア通信の際に優先して利用するコーデックを指定することができます。

**サンプルコード**

```ts
const video = await SkyWayMediaDevices.createCameraVideoStream();
await localMember.publish(video, {
  codecCapabilities: [{ mimeType: 'video/av1' }, { mimeType: 'video/h264' }],
});

const audio = await SkyWayMediaDevices.createMicrophoneAudioStream();
await localMember.publish(audio, {
  codecCapabilities: [{ mimeType: 'audio/red' }],
});
```

codecCapabilities 配列の先頭のコーデックを優先して利用します。
デバイスが先頭のコーデックに対応していない場合は後ろのコーデックを利用します。
どのコーデックにも対応していない場合はデバイスが対応している他のコーデックを自動的に利用します。

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

### マイク

```ts
const audio = await SkyWayMediaDevices.createMicrophoneAudioStream(options);
```

### カメラ

```ts
const video = await SkyWayMediaDevices.createCameraVideoStream(options);
```

### DataChannel

※SFU Room では使用できません。

```ts
const data = await SkyWayMediaDevices.createDataStream();
```

### MediaStreamTrack から AudioStream / VideoStream を作成する

任意の MediaStreamTrack から Stream を作成することが出来ます。

```ts
const displayStream = await navigator.mediaDevices.getDisplayMedia();
const [displayTrack] = displayStream.getVideoTracks();
const stream = new LocalVideoStream('label', displayTrack);

const [audioTrack] = (
  await navigator.mediaDevices.getUserMedia({ audio: true })
).getTracks();
const stream = new LocalAudioStream('label', audioTrack);
```

### AudioStream / VideoStream の利用方法

SkyWay の Stream を Html で再生する方法が 2 種類あります。

#### element に適用する

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

#### MediaStream を作る

MediaStream を作成して使うことが出来ます。

```ts
const stream = new MediaStream([
  // MediaStreamTrackにアクセスできる
  skywayStream.track,
]);
```

## Publication

Publication の情報の参照と Publication の操作ができます

### Metadata の更新

Publication に紐付いた Metadata を更新することができます

```ts
await publication.updateMetadata('metadata');
```

## Subscription

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

# Tips

## リモートの Member に Publication を Subscribe させる

Token の members scope を次のように設定することで、リモートの Member に任意の Publication を Subscribe させたり Unsubscribe させることができます。

```ts
const members = [
  {
    id: '*',
    name: '*',
    actions: ['write'],
    publication: {
      actions: ['write'],
    },
    subscription: {
      actions: ['write'],
    },
  },
];
```

**サンプルコード**

```ts
//...

const localMember: LocalRoomMember = await room.join({ name: 'alice' });

const video = await SkyWayMediaDevices.createCameraVideoStream();
const publication = await localMember.publish(video);

const remoteMember = room.members.find((member) => member.name === 'bob');
const remoteSubscription = await remoteMember.subscribe(publication);
```

リモートのメンバーの Subscription の stream を参照することはできません（stream プロパティの中身は常に undefined になります）
