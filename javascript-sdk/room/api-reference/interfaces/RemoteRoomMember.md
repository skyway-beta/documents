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

- [subscribe](RemoteRoomMember.md#subscribe)
- [unsubscribe](RemoteRoomMember.md#unsubscribe)
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

• `Readonly` **onLeft**: [`Event`](../classes/Event.md)<`void`\>

**`description`** {japanese} MemberがRoomから出たときに発火するイベント

#### Inherited from

[RoomMember](RoomMember.md).[onLeft](RoomMember.md#onleft)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

**`description`** {japanese} Memberのメタデータが更新された時に発火するイベント

#### Inherited from

[RoomMember](RoomMember.md).[onMetadataUpdated](RoomMember.md#onmetadataupdated)

___

### onPublicationSubscribed

• `Readonly` **onPublicationSubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemoteRoomMember がPublicationをSubscribeしたとき

___

### onPublicationUnsubscribed

• `Readonly` **onPublicationUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemoteRoomMember がPublicationをUnsubscribeしたとき

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} Memberが Publish した Publication のリスト

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

• `Readonly` **side**: ``"remote"``

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

[RoomMember](RoomMember.md).[status](RoomMember.md#status)

___

### subscriptions

• `Readonly` **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

**`description`** {japanese} Memberが Subscribe している Subscription のリスト

#### Inherited from

[RoomMember](RoomMember.md).[subscriptions](RoomMember.md#subscriptions)

## Methods

### subscribe

▸ **subscribe**(`publicationId`): `Promise`<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemoteRoomMember にPublicationをSubscribeさせる

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

___

### unsubscribe

▸ **unsubscribe**(`subscriptionId`): `Promise`<`void`\>

**`description`** {japanese} この RemoteRoomMember にPublicationをUnsubscribeさせる

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Promise`<`void`\>

___

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

**`description`** {japanese} Memberのメタデータを更新する

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[RoomMember](RoomMember.md).[updateMetadata](RoomMember.md#updatemetadata)
