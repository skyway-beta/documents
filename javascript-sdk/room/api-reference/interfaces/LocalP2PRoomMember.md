[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalP2PRoomMember

# Interface: LocalP2PRoomMember

## Hierarchy

- [`LocalRoomMember`](LocalRoomMember.md)

  ↳ **`LocalP2PRoomMember`**

## Table of contents

### Properties

- [id](LocalP2PRoomMember.md#id)
- [metadata](LocalP2PRoomMember.md#metadata)
- [name](LocalP2PRoomMember.md#name)
- [onLeft](LocalP2PRoomMember.md#onleft)
- [onMetadataUpdated](LocalP2PRoomMember.md#onmetadataupdated)
- [onPublicationChanged](LocalP2PRoomMember.md#onpublicationchanged)
- [onStreamPublished](LocalP2PRoomMember.md#onstreampublished)
- [onStreamSubscribed](LocalP2PRoomMember.md#onstreamsubscribed)
- [onStreamUnpublished](LocalP2PRoomMember.md#onstreamunpublished)
- [onStreamUnsubscribed](LocalP2PRoomMember.md#onstreamunsubscribed)
- [onSubscriptionChanged](LocalP2PRoomMember.md#onsubscriptionchanged)
- [publications](LocalP2PRoomMember.md#publications)
- [room](LocalP2PRoomMember.md#room)
- [roomId](LocalP2PRoomMember.md#roomid)
- [roomName](LocalP2PRoomMember.md#roomname)
- [roomType](LocalP2PRoomMember.md#roomtype)
- [side](LocalP2PRoomMember.md#side)
- [status](LocalP2PRoomMember.md#status)
- [subscriptions](LocalP2PRoomMember.md#subscriptions)

### Methods

- [leave](LocalP2PRoomMember.md#leave)
- [publish](LocalP2PRoomMember.md#publish)
- [subscribe](LocalP2PRoomMember.md#subscribe)
- [unpublish](LocalP2PRoomMember.md#unpublish)
- [unsubscribe](LocalP2PRoomMember.md#unsubscribe)
- [updateMetadata](LocalP2PRoomMember.md#updatemetadata)

## Properties

### id

• `Readonly` **id**: `string`

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[id](LocalRoomMember.md#id)

___

### metadata

• `Optional` `Readonly` **metadata**: `string`

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[metadata](LocalRoomMember.md#metadata)

___

### name

• `Optional` `Readonly` **name**: `string`

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[name](LocalRoomMember.md#name)

___

### onLeft

• `Readonly` **onLeft**: [`Event`](../classes/Event.md)<`void`\>

**`description`** {japanese} MemberがRoomから出たときに発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onLeft](LocalRoomMember.md#onleft)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

**`description`** {japanese} Memberのメタデータが更新された時に発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onMetadataUpdated](LocalRoomMember.md#onmetadataupdated)

___

### onPublicationChanged

• **onPublicationChanged**: [`Event`](../classes/Event.md)<`void`\>

**`description`** {japanese} このMemberがStreamをSubscribeしたときに発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onPublicationChanged](LocalRoomMember.md#onpublicationchanged)

___

### onStreamPublished

• **onStreamPublished**: [`Event`](../classes/Event.md)<{ `publication`: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このMemberがStreamをPublishしたときに発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onStreamPublished](LocalRoomMember.md#onstreampublished)

___

### onStreamSubscribed

• **onStreamSubscribed**: [`Event`](../classes/Event.md)<{ `stream`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このMemberがStreamをSubscribeしたときに発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onStreamSubscribed](LocalRoomMember.md#onstreamsubscribed)

___

### onStreamUnpublished

• **onStreamUnpublished**: [`Event`](../classes/Event.md)<{ `publication`: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このMemberがStreamをUnPublishしたときに発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onStreamUnpublished](LocalRoomMember.md#onstreamunpublished)

___

### onStreamUnsubscribed

• **onStreamUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このMemberがStreamをUnsubscribeしたときに発火するイベント

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onStreamUnsubscribed](LocalRoomMember.md#onstreamunsubscribed)

___

### onSubscriptionChanged

• **onSubscriptionChanged**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[onSubscriptionChanged](LocalRoomMember.md#onsubscriptionchanged)

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} Memberが Publish した Publication のリスト

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[publications](LocalRoomMember.md#publications)

___

### room

• **room**: [`Room`](Room.md)

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[room](LocalRoomMember.md#room)

___

### roomId

• `Readonly` **roomId**: `string`

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[roomId](LocalRoomMember.md#roomid)

___

### roomName

• `Optional` `Readonly` **roomName**: `string`

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[roomName](LocalRoomMember.md#roomname)

___

### roomType

• `Readonly` **roomType**: ``"sfu"`` \| ``"p2p"``

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[roomType](LocalRoomMember.md#roomtype)

___

### side

• **side**: ``"local"``

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[side](LocalRoomMember.md#side)

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[status](LocalRoomMember.md#status)

___

### subscriptions

• `Readonly` **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

**`description`** {japanese} Memberが Subscribe している Subscription のリスト

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[subscriptions](LocalRoomMember.md#subscriptions)

## Methods

### leave

▸ **leave**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[leave](LocalRoomMember.md#leave)

___

### publish

▸ **publish**<`T`\>(`stream`, `options?`): `Promise`<[`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>\>

**`description`** {japanese} StreamをPublishする

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`LocalStream`](../modules.md#localstream) = [`LocalStream`](../modules.md#localstream) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `stream` | `T` |
| `options?` | `PublicationOptions` |

#### Returns

`Promise`<[`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>\>

___

### subscribe

▸ **subscribe**<`T`\>(`publicationId`): `Promise`<{ `stream`: `T` ; `subscription`: [`RoomSubscription`](RoomSubscription.md)<`T`\>  }\>

**`description`** {japanese} StreamのPublicationをSubscribeする

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`RemoteStream`](../modules.md#remotestream) = [`RemoteStream`](../modules.md#remotestream) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<{ `stream`: `T` ; `subscription`: [`RoomSubscription`](RoomSubscription.md)<`T`\>  }\>

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[subscribe](LocalRoomMember.md#subscribe)

___

### unpublish

▸ **unpublish**(`publicationId`): `Promise`<`void`\>

**`description`** {japanese} StreamのPublicationをUnpublishする

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[unpublish](LocalRoomMember.md#unpublish)

___

### unsubscribe

▸ **unsubscribe**(`subscriptionId`): `Promise`<`void`\>

**`description`** {japanese} StreamのSubscriptionをUnsubscribeする

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[LocalRoomMember](LocalRoomMember.md).[unsubscribe](LocalRoomMember.md#unsubscribe)

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

[LocalRoomMember](LocalRoomMember.md).[updateMetadata](LocalRoomMember.md#updatemetadata)
