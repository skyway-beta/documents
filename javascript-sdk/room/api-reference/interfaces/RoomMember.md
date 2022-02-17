[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / RoomMember

# Interface: RoomMember

## Hierarchy

- **`RoomMember`**

  ↳ [`LocalRoomMember`](LocalRoomMember.md)

  ↳ [`RemoteRoomMember`](RemoteRoomMember.md)

## Table of contents

### Properties

- [id](RoomMember.md#id)
- [metadata](RoomMember.md#metadata)
- [name](RoomMember.md#name)
- [onLeft](RoomMember.md#onleft)
- [onMetadataUpdated](RoomMember.md#onmetadataupdated)
- [publications](RoomMember.md#publications)
- [roomId](RoomMember.md#roomid)
- [roomName](RoomMember.md#roomname)
- [roomType](RoomMember.md#roomtype)
- [status](RoomMember.md#status)
- [subscriptions](RoomMember.md#subscriptions)

### Methods

- [updateMetadata](RoomMember.md#updatemetadata)

## Properties

### id

• `Readonly` **id**: `string`

___

### metadata

• `Optional` `Readonly` **metadata**: `string`

___

### name

• `Optional` `Readonly` **name**: `string`

___

### onLeft

• `Readonly` **onLeft**: `Event`<`void`\>

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<`string`\>

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

___

### roomId

• `Readonly` **roomId**: `string`

___

### roomName

• `Optional` `Readonly` **roomName**: `string`

___

### roomType

• `Readonly` **roomType**: ``"sfu"`` \| ``"p2p"``

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

___

### subscriptions

• `Readonly` **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

## Methods

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>
