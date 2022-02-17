# SFU Client SDK

SkyWay Core SDK で SFU Bot を利用するためのプラグイン です。

# インストール方法

```sh
npm i @skyway-nv/sfu-client
```

# SFU Bot のしくみ

P2P での WebRTC は、各 PersonMember が通信したい各 PersonMember に対してそれぞれデータの配信を行う必要があるので、 PersonMember 数が増えてくると各 PersonMember の上りのトラフィックコストとメディアのエンコード処理がボトルネックになります。

SFU Bot は、 PersonMember から一本の上りトラフィックを受信し、代わりに他の PersonMember に対してそれを配信することで、クライアントの負荷を軽減し、大規模な WebRTC 利用を可能にします。

# 利用方法

## プラグインの登録

Core SDK で SFU 機能を有効化するために Plugin を Core SDK に登録する必要があります。

```ts
import { SkyWayContext } from '@skyway-nv/core';
import { registerSfuPlugin } from '@skyway-nv/sfu-client';

const context = await SkyWayContext.Create('token');
const plugin = new SfuClientPlugin();
context.registerPlugin(plugin);
```

## SFU Bot の呼び出し

Channel で SFU Bot を利用するために、対象の Channel に SFU Bot を呼び出す必要があります。

```ts
const context = await SkyWayContext.Create('token');
const plugin = new SfuClientPlugin();
context.registerPlugin(plugin);

const channel = await Channel.FindOrCreate(context, { name: 'test' });
// SFU BotをChannelに呼び出す。
const bot = await plugin.createBot(channel);
```

## Publication の Forwarding

SFU Bot に Channel 上の Publication を Forwarding させます。

これにより、SFU Bot は、 PersonMember から一本の上りトラフィックを受信し、代わりに他の PersonMember に対してそれを配信します。

```ts
const person = await channel.join();

const stream = await MediaDevices.createCameraVideoStream();
const publication = await person.publish(stream);

// PersonMemberがPublishしたStreamのPublicationをSFU BotにForwardingさせる
const forwarding = await bot.startForwarding(publication);
```

PersonMember は SFU Bot が Forwarding している Publication を Subscribe することで、SFU 経由で Stream を受け取ることができます。

## Publication の種類の見分け方

SFU Bot を利用する場合、Channel 上には PersonMember が Publish した Publication と SFU Bot がその Publication を Forwarding している Publication の 2 種類の Publication が存在します。

PersonMember が SFU Bot 経由で配信されている Publication だけを Subscribe する方法について説明します。

```ts
channel.onStreamPublished.add(({ publication }) => {
  if (publication.publisher.subtype === 'sfu') {
    console.log('published by SFU');
    person.subscribe(publication.id);
  }
});
```

Publication の Publisher の SubType から Publication の Publisher の種類を識別できます。
