# Core SDK

SkyWay を使うために必要な基本的な要素（Channel, Member, Stream, ...）を提供する SDK です。
Room SDK でカバーできないような、SkyWay によって提供される機能をより細かに制御し最大限に利用したいユースケースに向いています。

# インストール方法

```sh
npm i @skyway-nv/core
```

# 概要

アプリケーションのクライアントはメディア通信を開始するまでに次のようなフローをたどります。

**1. Token を入手する**

SkyWay サービスはユーザの認証認可に独自の JWT Token を使用しています。
この Token は 2 種類の方法で入手することができます。

- アプリケーションサーバサイドで生成したトークンをクライアントで使用する
- クライアント上でトークンを生成して使用する

後者の方法だと正しく権限の制限をすることができないので前者の方法を取ることを推奨します。

**2. Channel を作成する**

メディア通信を行うグループの単位を Channel と呼びます。
メディア通信を開始するにはまず Channel を作る権限を持った Token を用いて Channel を作成する必要があります。

**3. クライアントが Channel に Join して Channel の Member となる**

この際に Channel に参加する権限を持った Token とともに Channel に Join する必要があります

**4. メディアの Stream を Channel 内に Publish および Subscribe する**

Member が Stream を Publish すると Channel 上に Stream の情報である Publication というリソースが生成されます。

他の Member はこの Publication を Subscribe すると Subscription というリソースが Channel 上に生成され、Subscription に対応する Stream を受信し、メディア通信が開始できます。

# 用語解説

Core SDK の用語、仕様について説明します。

## Channel

複数の Member が通信するグループの単位です。

それぞれの Member は Channel 内にいる他の Member と映像/音声/データの送受信が出来ます。

### Channel ID

Channel ID は SkyWay サービスによって設定される Channel を一意に識別するための ID です。

### Channel Name

Channel Name はユーザが Channel を作成する際に指定することができる任意の値です。

アプリケーション内で重複した Channel Name を指定することはできません。

## Member

Member は他のクライアントとの通信を管理するエージェントです。

映像や音声を送信したり、受信したりすることが出来ます。

Member は大きく Person と Bot の 2 種類に分類されます。

**Person**

Person は Core SDK を使って Channel に参加し通信を行う Member です。

**Bot**

Bot は SFU Bot や Recording Bot といった SkyWay サービス側が提供する特殊な Member です。Bot は個別のプラグインパッケージとして提供され、利用できます。

### Member ID

Member ID は SkyWay サービスによって設定される Member を一意に識別するための ID です。

### Member Name

Member Name はクライアントが Channel に Join する際に指定することができる任意の値です。

Channel 内で重複した Member Name を指定することはできません。

## Stream

Channel 内で Member が通信するメディアのことを Stream と呼びます。

三種類の Stream が存在します。

- VideoStream
- AudioStream
- DataStream

## Publication

あるクライアントが用意した Stream を他の Member が受信可能にするために Channel 内に公開する操作のことを Publish と呼びます。Stream を Publish すると Channel 内に Publication というリソースが生成されます。

他の Member は Publication を Subscribe することで Subscription というリソースを得られて、Stream の受信が開始されます。

Publication を Unpublish すると SkyWay サービス側で関連する Subscription を Unsubscribe して削除します。

## Subscription

あるクライアントが Channel に存在する Publication を Subscribe した時に得られるリソースです。Subscription には Stream が含まれており、メディアの受信が可能です。

Channel 内の Subscription を見ることでどの Member がどの Publication を Subscribe しているかを把握することができます。

クライアントの Member が Subscribe していない Subscription の Stream を参照することはできません。Member が Stream を受信するためには必ずその Member が Publication を Subscribe して Subscription を作る必要があります。

Subscription と紐ついている Publication が Unpublish されると Subscription は自動的に Unsubscribe されます。

## Plugin

SkyWay の Core SDK では SFU や録音録画機能を Bot という形で提供しています。

Plugin はこの Sfu Bot や Recording Bot などの Bot を利用するための仕組みです。

各 Plugin の使い方は各 Plugin のドキュメントに記載されています。

# クラス一覧

- SkyWayContext
- Channel
- LocalPerson
- SkyWayMediaDevices
- Publication
- Subscription

## SkyWayContext

アプリケーションの設定を行います。

```ts
import { SkyWayContext } from '@skyway-nv/core';

const context = await SkyWayContext.Create(tokenString);
```

事前にトークンの取得が必要になります。

### トークンの取得方法

SkyWay サービスの JWT トークンはトークンの仕様に基づいて自身で作成するか、`@skyway-nv/token`ライブラリを使って作成することができます。

`@skyway-nv/token`ライブラリは Node.js サーバとブラウザで動作しますが、トークンでユーザの行動を制限したい場合は必ずサーバ側でトークンを作成して下さい。

```ts
import { SkyWayAuthToken } from '@skyway-nv/token';

const token = new SkyWayAuthToken(parameters);
const tokenString = token.encode('secret');
```

## Channel

Member の参加する Channel の作成/取得を行います。

**作成**

新しい Channel を作成します。

```ts
import { SkyWayContext, Channel } from '@skyway-nv/core';

const context = await SkyWayContext.Create(tokenString);
const channel = await Channel.Create(context, {
  name: 'something',
  metadata: 'something',
});
```

作成時に`name`と`metadata`の設定が可能です。(optional)
`name`は App 内の他の Channel と重複することはできません。

**取得**

既存の Channel を取得します。

```ts
import { SkyWayContext, Channel } from '@skyway-nv/core';

const context = await SkyWayContext.Create(tokenString);
const channel = await Channel.Find(context, {
  id: 'uuid',
  name: 'something',
});
```

id か name を使って Channel を探すことができます。

**取得もしくは作成**

Channel の取得を試み、存在しなければ作成します。

```ts
import { SkyWayContext, Channel } from '@skyway-nv/core';

const context = await SkyWayContext.Create(tokenString);
const channel = await Channel.FindOrCreate(context, { name: 'channelName' });
```

### Channel に LocalPerson を追加する

```ts
const person: LocalPerson = await channel.join({
  name: 'something',
  metadata: 'something',
});
```

追加時に`name`と`metadata`の設定が可能です。(optional)
`name`は Channel 内の他の Member と重複することはできません。

### Channel の情報にアクセスする

**Member**

Stream の Member の情報のリストを参照することが出来ます。

```ts
const members = channel.members;
```

**Publication**

Stream の Publication のリストを参照することが出来ます。

```ts
const publications = channel.publications;
```

**Subscription**

Stream の Subscription のリストを参照することが出来ます。

```ts
const subscriptions = channel.subscriptions;
```

## LocalPerson

Stream の Publish、Subscribe などを行うことが出来ます。

### Stream の Publish

Channel に Stream を Publish することができます。

```ts
import { SkyWayMediaDevices } from '@skyway-nv/channel';

...

const video = await SkyWayMediaDevices.createCameraVideoStream();
const publication = await person.publish(video,options);
```

以下のオプションが指定可能です。

```ts
interface Option {
  metadata?: string | undefined;
  codecCapabilities?: Codec[];
  encodings?: EncodingParameters[];
}
```

### Stream の Unpublish

Channel 上の Stream の Publication を Unpublish することができます。
関連する Subscription が自動的に Unsubscribe されます。

```ts
await person.unpublish(publication.id);
```

### Stream の Subscribe

Channel 上の Stream の Publication を Subscribe することができます。

```ts
const { subscription, stream } = await person.subscribe(publication.id);
```

### Stream の Unsubscribe

Subscribe している Stream の Subscription を Unsubscribe することができます。

```ts
await person.unsubscribe(subscription.id);
```

### Metadata の更新

Member に紐付いた Metadata を更新することができます

```ts
await person.updateMetadata('metadata');
```

## SkyWayMediaDevices

各種 Stream の取得が出来ます。

**マイク**

```ts
const audio: LocalAudioStream =
  await SkyWayMediaDevices.createMicrophoneAudioStream(options);
```

**カメラ**

```ts
const video: LocalVideoStream =
  await SkyWayMediaDevices.createCameraVideoStream(options);
```

**DataChannel**

```ts
const data: LocalDataStream = await SkyWayMediaDevices.createDataStream();
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