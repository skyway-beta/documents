[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / P2PConnection

# Class: P2PConnection

## Implements

- [`SkyWayConnection`](../interfaces/SkyWayConnection.md)

## Table of contents

### Constructors

- [constructor](P2PConnection.md#constructor)

### Properties

- [channelId](P2PConnection.md#channelid)
- [closed](P2PConnection.md#closed)
- [disconnected](P2PConnection.md#disconnected)
- [localPersonId](P2PConnection.md#localpersonid)
- [onClose](P2PConnection.md#onclose)
- [onDisconnect](P2PConnection.md#ondisconnect)
- [receiver](P2PConnection.md#receiver)
- [remoteMember](P2PConnection.md#remotemember)
- [sender](P2PConnection.md#sender)
- [type](P2PConnection.md#type)

### Methods

- [close](P2PConnection.md#close)
- [getStats](P2PConnection.md#getstats)
- [startPublishing](P2PConnection.md#startpublishing)
- [startSubscribing](P2PConnection.md#startsubscribing)
- [stopPublishing](P2PConnection.md#stoppublishing)
- [stopSubscribing](P2PConnection.md#stopsubscribing)

## Constructors

### constructor

• **new P2PConnection**(`_iceManager`, `_messenger`, `channelId`, `localPersonId`, `remoteMember`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_iceManager` | `IceManager` |
| `_messenger` | `P2PMessenger` |
| `channelId` | `string` |
| `localPersonId` | `string` |
| `remoteMember` | `Pick`<[`Member`](../interfaces/Member.md), ``"name"`` \| ``"id"``\> |

## Properties

### channelId

• `Readonly` **channelId**: `string`

___

### closed

• **closed**: `boolean` = `false`

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[closed](../interfaces/SkyWayConnection.md#closed)

___

### disconnected

• **disconnected**: `boolean` = `false`

___

### localPersonId

• `Readonly` **localPersonId**: `string`

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[localPersonId](../interfaces/SkyWayConnection.md#localpersonid)

___

### onClose

• `Readonly` **onClose**: [`Event`](Event.md)<`void`\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[onClose](../interfaces/SkyWayConnection.md#onclose)

___

### onDisconnect

• `Readonly` **onDisconnect**: [`Event`](Event.md)<`void`\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[onDisconnect](../interfaces/SkyWayConnection.md#ondisconnect)

___

### receiver

• `Readonly` **receiver**: `Receiver`

___

### remoteMember

• `Readonly` **remoteMember**: `Pick`<[`Member`](../interfaces/Member.md), ``"name"`` \| ``"id"``\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[remoteMember](../interfaces/SkyWayConnection.md#remotemember)

___

### sender

• `Readonly` **sender**: `Sender`

___

### type

• `Readonly` **type**: ``"p2p"``

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[type](../interfaces/SkyWayConnection.md#type)

## Methods

### close

▸ **close**(): `void`

#### Returns

`void`

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[close](../interfaces/SkyWayConnection.md#close)

___

### getStats

▸ **getStats**(`content`): `Promise`<`RTCStatsReport`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `content` | [`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\> \| [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\> |

#### Returns

`Promise`<`RTCStatsReport`\>

___

### startPublishing

▸ **startPublishing**(`publication`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `PublicationImpl`<[`LocalStream`](../modules.md#localstream)\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[startPublishing](../interfaces/SkyWayConnection.md#startpublishing)

___

### startSubscribing

▸ **startSubscribing**(`subscription`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | `SubscriptionImpl`<[`RemoteStream`](../modules.md#remotestream)\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[startSubscribing](../interfaces/SkyWayConnection.md#startsubscribing)

___

### stopPublishing

▸ **stopPublishing**(`publication`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | [`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[stopPublishing](../interfaces/SkyWayConnection.md#stoppublishing)

___

### stopSubscribing

▸ **stopSubscribing**(`subscription`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[stopSubscribing](../interfaces/SkyWayConnection.md#stopsubscribing)
