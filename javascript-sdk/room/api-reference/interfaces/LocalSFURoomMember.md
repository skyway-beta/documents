[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalSFURoomMember

# Interface: LocalSFURoomMember

## Hierarchy

- [`LocalRoomMember`](LocalRoomMember.md)

  ↳ **`LocalSFURoomMember`**

## Table of contents

### Properties

- [id](LocalSFURoomMember.md#id)
- [metadata](LocalSFURoomMember.md#metadata)
- [name](LocalSFURoomMember.md#name)
- [onLeft](LocalSFURoomMember.md#onleft)
- [onMetadataUpdated](LocalSFURoomMember.md#onmetadataupdated)
- [onPublicationChanged](LocalSFURoomMember.md#onpublicationchanged)
- [onStreamPublished](LocalSFURoomMember.md#onstreampublished)
- [onStreamSubscribed](LocalSFURoomMember.md#onstreamsubscribed)
- [onStreamUnpublished](LocalSFURoomMember.md#onstreamunpublished)
- [onStreamUnsubscribed](LocalSFURoomMember.md#onstreamunsubscribed)
- [onSubscriptionChanged](LocalSFURoomMember.md#onsubscriptionchanged)
- [publications](LocalSFURoomMember.md#publications)
- [room](LocalSFURoomMember.md#room)
- [roomId](LocalSFURoomMember.md#roomid)
- [roomName](LocalSFURoomMember.md#roomname)
- [roomType](LocalSFURoomMember.md#roomtype)
- [side](LocalSFURoomMember.md#side)
- [status](LocalSFURoomMember.md#status)
- [subscriptions](LocalSFURoomMember.md#subscriptions)

### Methods

- [leave](LocalSFURoomMember.md#leave)
- [publish](LocalSFURoomMember.md#publish)
- [subscribe](LocalSFURoomMember.md#subscribe)
- [unpublish](LocalSFURoomMember.md#unpublish)
- [unsubscribe](LocalSFURoomMember.md#unsubscribe)
- [updateMetadata](LocalSFURoomMember.md#updatemetadata)

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

▸ **publish**(`stream`, `options?`): `Promise`<[`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>\>

**`description`** {japanese} RoomにStreamをPublishする

#### Parameters

| Name | Type |
| :------ | :------ |
| `stream` | [`LocalStream`](../modules.md#localstream) |
| `options?` | `PublicationOptions` & [`SfuRoomPublicationOptions`](SfuRoomPublicationOptions.md) |

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
| `publicationId` | `string` \| [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\> |

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
| `publicationId` | `string` \| [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\> |

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
| `subscriptionId` | `string` \| [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\> |

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
