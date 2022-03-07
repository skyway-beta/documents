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

• `Readonly` **onLeft**: [`Event`](../classes/Event.md)<`void`\>

**`description`** {japanese} MemberがRoomから出たときに発火するイベント

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

**`description`** {japanese} Memberのメタデータが更新された時に発火するイベント

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} Memberが Publish した Publication のリスト

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

**`description`** {japanese} Memberが Subscribe している Subscription のリスト

## Methods

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

**`description`** {japanese} Memberのメタデータを更新する

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>
