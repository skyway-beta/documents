[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayConnection

# Interface: SkyWayConnection

## Implemented by

- [`P2PConnection`](../classes/P2PConnection.md)

## Table of contents

### Properties

- [closed](SkyWayConnection.md#closed)
- [localPersonId](SkyWayConnection.md#localpersonid)
- [onClose](SkyWayConnection.md#onclose)
- [onDisconnect](SkyWayConnection.md#ondisconnect)
- [remoteMember](SkyWayConnection.md#remotemember)
- [type](SkyWayConnection.md#type)

### Methods

- [close](SkyWayConnection.md#close)
- [startPublishing](SkyWayConnection.md#startpublishing)
- [startSubscribing](SkyWayConnection.md#startsubscribing)
- [stopPublishing](SkyWayConnection.md#stoppublishing)
- [stopSubscribing](SkyWayConnection.md#stopsubscribing)

## Properties

### closed

• **closed**: `boolean`

___

### localPersonId

• `Readonly` **localPersonId**: `string`

___

### onClose

• `Readonly` **onClose**: [`Event`](../classes/Event.md)<`void`\>

___

### onDisconnect

• `Readonly` **onDisconnect**: [`Event`](../classes/Event.md)<`void`\>

___

### remoteMember

• `Readonly` **remoteMember**: `Pick`<[`Member`](Member.md), ``"name"`` \| ``"id"``\>

___

### type

• `Readonly` **type**: `string`

## Methods

### close

▸ **close**(): `void`

#### Returns

`void`

___

### startPublishing

▸ `Optional` **startPublishing**(`publication`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `PublicationImpl`<[`LocalStream`](../modules.md#localstream)\> |

#### Returns

`Promise`<`void`\>

___

### startSubscribing

▸ `Optional` **startSubscribing**(`subscription`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | `SubscriptionImpl`<[`RemoteStream`](../modules.md#remotestream)\> |

#### Returns

`Promise`<`void`\>

___

### stopPublishing

▸ `Optional` **stopPublishing**(`publication`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `PublicationImpl`<[`LocalStream`](../modules.md#localstream)\> |

#### Returns

`Promise`<`void`\>

___

### stopSubscribing

▸ `Optional` **stopSubscribing**(`subscription`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | `SubscriptionImpl`<[`RemoteStream`](../modules.md#remotestream)\> |

#### Returns

`Promise`<`void`\>
