[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / RemoteRoomMember

# Interface: RemoteRoomMember

## Hierarchy

- [`RoomMember`](RoomMember.md)

  ↳ **`RemoteRoomMember`**

## Table of contents

### Properties

- [id](RemoteRoomMember.md#id)
- [metadata](RemoteRoomMember.md#metadata)
- [name](RemoteRoomMember.md#name)
- [onLeft](RemoteRoomMember.md#onleft)
- [onMetadataUpdated](RemoteRoomMember.md#onmetadataupdated)
- [onPublicationSubscribed](RemoteRoomMember.md#onpublicationsubscribed)
- [onPublicationUnsubscribed](RemoteRoomMember.md#onpublicationunsubscribed)
- [publications](RemoteRoomMember.md#publications)
- [roomId](RemoteRoomMember.md#roomid)
- [roomName](RemoteRoomMember.md#roomname)
- [roomType](RemoteRoomMember.md#roomtype)
- [side](RemoteRoomMember.md#side)
- [status](RemoteRoomMember.md#status)
- [subscriptions](RemoteRoomMember.md#subscriptions)

### Methods

- [updateMetadata](RemoteRoomMember.md#updatemetadata)

## Properties

### id

• `Readonly` **id**: `string`

#### Inherited from

[RoomMember](RoomMember.md).[id](RoomMember.md#id)

___

### metadata

• `Optional` `Readonly` **metadata**: `string`

#### Inherited from

[RoomMember](RoomMember.md).[metadata](RoomMember.md#metadata)

___

### name

• `Optional` `Readonly` **name**: `string`

#### Inherited from

[RoomMember](RoomMember.md).[name](RoomMember.md#name)

___

### onLeft

• `Readonly` **onLeft**: `Event`<`void`\>

#### Inherited from

[RoomMember](RoomMember.md).[onLeft](RoomMember.md#onleft)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<`string`\>

#### Inherited from

[RoomMember](RoomMember.md).[onMetadataUpdated](RoomMember.md#onmetadataupdated)

___

### onPublicationSubscribed

• **onPublicationSubscribed**: `Event`<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

___

### onPublicationUnsubscribed

• **onPublicationUnsubscribed**: `Event`<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

[RoomMember](RoomMember.md).[publications](RoomMember.md#publications)

___

### roomId

• `Readonly` **roomId**: `string`

#### Inherited from

[RoomMember](RoomMember.md).[roomId](RoomMember.md#roomid)

___

### roomName

• `Optional` `Readonly` **roomName**: `string`

#### Inherited from

[RoomMember](RoomMember.md).[roomName](RoomMember.md#roomname)

___

### roomType

• `Readonly` **roomType**: ``"sfu"`` \| ``"p2p"``

#### Inherited from

[RoomMember](RoomMember.md).[roomType](RoomMember.md#roomtype)

___

### side

• **side**: ``"remote"``

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

[RoomMember](RoomMember.md).[status](RoomMember.md#status)

___

### subscriptions

• `Readonly` **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Inherited from

[RoomMember](RoomMember.md).[subscriptions](RoomMember.md#subscriptions)

## Methods

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[RoomMember](RoomMember.md).[updateMetadata](RoomMember.md#updatemetadata)
