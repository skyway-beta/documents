[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayChannel

# Class: SkyWayChannel

## Table of contents

### Methods

- [Create](SkyWayChannel.md#create)
- [Find](SkyWayChannel.md#find)
- [FindOrCreate](SkyWayChannel.md#findorcreate)

## Methods

### Create

▸ `Static` **Create**(`context`, `init?`): `Promise`<[`Channel`](../interfaces/Channel.md)\>

**`description`** {japanese} Channelの作成

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `init` | [`ChannelInit`](../interfaces/ChannelInit.md) |

#### Returns

`Promise`<[`Channel`](../interfaces/Channel.md)\>

___

### Find

▸ `Static` **Find**(`context`, `query`): `Promise`<[`Channel`](../interfaces/Channel.md)\>

**`description`** {japanese} 既存のChannelの取得

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `query` | [`ChannelQuery`](../interfaces/ChannelQuery.md) |

#### Returns

`Promise`<[`Channel`](../interfaces/Channel.md)\>

___

### FindOrCreate

▸ `Static` **FindOrCreate**(`context`, `query`): `Promise`<[`Channel`](../interfaces/Channel.md)\>

**`description`** {japanese} Channelの取得を試み、存在しなければ作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `query` | [`ChannelInit`](../interfaces/ChannelInit.md) |

#### Returns

`Promise`<[`Channel`](../interfaces/Channel.md)\>
