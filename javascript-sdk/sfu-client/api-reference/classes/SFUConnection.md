[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / SFUConnection

# Class: SFUConnection

## Implements

- `SkyWayConnection`

## Table of contents

### Constructors

- [constructor](SFUConnection.md#constructor)

### Properties

- [channelId](SFUConnection.md#channelid)
- [closed](SFUConnection.md#closed)
- [localPersonId](SFUConnection.md#localpersonid)
- [onClose](SFUConnection.md#onclose)
- [onDisconnect](SFUConnection.md#ondisconnect)
- [remoteMember](SFUConnection.md#remotemember)
- [type](SFUConnection.md#type)

### Methods

- [addSenderConnection](SFUConnection.md#addsenderconnection)
- [close](SFUConnection.md#close)
- [getReceiver](SFUConnection.md#getreceiver)
- [getSender](SFUConnection.md#getsender)
- [removeSenderConnection](SFUConnection.md#removesenderconnection)
- [startSubscribing](SFUConnection.md#startsubscribing)
- [stopPublishing](SFUConnection.md#stoppublishing)
- [stopSubscribing](SFUConnection.md#stopsubscribing)

## Constructors

### constructor

• **new SFUConnection**(`_iceManager`, `_api`, `channelId`, `localPersonId`, `remoteMember`, `_context`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_iceManager` | `IceManager` |
| `_api` | `SfuRestApiClient` |
| `channelId` | `string` |
| `localPersonId` | `string` |
| `remoteMember` | `Member` |
| `_context` | `SkyWayContext` |

## Properties

### channelId

• `Readonly` **channelId**: `string`

___

### closed

• **closed**: `boolean` = `false`

#### Implementation of

SkyWayConnection.closed

___

### localPersonId

• `Readonly` **localPersonId**: `string`

#### Implementation of

SkyWayConnection.localPersonId

___

### onClose

• `Readonly` **onClose**: `Event`<`void`\>

#### Implementation of

SkyWayConnection.onClose

___

### onDisconnect

• `Readonly` **onDisconnect**: `Event`<`void`\>

#### Implementation of

SkyWayConnection.onDisconnect

___

### remoteMember

• `Readonly` **remoteMember**: `Member`

#### Implementation of

SkyWayConnection.remoteMember

___

### type

• `Readonly` **type**: ``"sfu"``

#### Implementation of

SkyWayConnection.type

## Methods

### addSenderConnection

▸ **addSenderConnection**(`publication`): `Sender`

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `PublicationImpl`<`LocalVideoStream` \| `LocalAudioStream`\> |

#### Returns

`Sender`

___

### close

▸ **close**(): `void`

#### Returns

`void`

#### Implementation of

SkyWayConnection.close

___

### getReceiver

▸ **getReceiver**(`subscriptionId`): `Receiver`

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Receiver`

___

### getSender

▸ **getSender**(`forwardingId`): `Sender`

#### Parameters

| Name | Type |
| :------ | :------ |
| `forwardingId` | `string` |

#### Returns

`Sender`

___

### removeSenderConnection

▸ **removeSenderConnection**(`originPublicationId`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `originPublicationId` | `string` |

#### Returns

`void`

___

### startSubscribing

▸ **startSubscribing**(`subscription`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | `SubscriptionImpl`<`RemoteStream`\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

SkyWayConnection.startSubscribing

___

### stopPublishing

▸ **stopPublishing**(`publication`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `Publication`<`LocalStream`\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

SkyWayConnection.stopPublishing

___

### stopSubscribing

▸ **stopSubscribing**(`subscription`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | `Subscription`<`RemoteStream`\> |

#### Returns

`Promise`<`void`\>

#### Implementation of

SkyWayConnection.stopSubscribing
