[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / P2PConnection

# Class: P2PConnection

## Implements

- [`SkyWayConnection`](../interfaces/SkyWayConnection.md)

## Table of contents

### Properties

- [channelId](P2PConnection.md#channelid)
- [closed](P2PConnection.md#closed)
- [disconnected](P2PConnection.md#disconnected)
- [localPerson](P2PConnection.md#localperson)
- [onClose](P2PConnection.md#onclose)
- [onDisconnect](P2PConnection.md#ondisconnect)
- [receiver](P2PConnection.md#receiver)
- [remoteMember](P2PConnection.md#remotemember)
- [sender](P2PConnection.md#sender)
- [type](P2PConnection.md#type)

### Methods

- [getStats](P2PConnection.md#getstats)

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

### localPerson

• `Readonly` **localPerson**: `LocalPersonImpl`

#### Implementation of

[SkyWayConnection](../interfaces/SkyWayConnection.md).[localPerson](../interfaces/SkyWayConnection.md#localperson)

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

• `Readonly` **remoteMember**: `Pick`<[`Member`](../interfaces/Member.md), ``"id"`` \| ``"name"``\>

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

### getStats

▸ **getStats**(`content`): `Promise`<`RTCStatsReport`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `content` | [`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\> \| [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\> |

#### Returns

`Promise`<`RTCStatsReport`\>
