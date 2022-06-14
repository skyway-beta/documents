[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalRoomMember

# Interface: LocalRoomMember

## Hierarchy

- [`RoomMember`](RoomMember.md)

  ↳ **`LocalRoomMember`**

  ↳↳ [`LocalP2PRoomMember`](LocalP2PRoomMember.md)

  ↳↳ [`LocalSFURoomMember`](LocalSFURoomMember.md)

## Table of contents

### Properties

- [id](LocalRoomMember.md#id)
- [metadata](LocalRoomMember.md#metadata)
- [name](LocalRoomMember.md#name)
- [onLeft](LocalRoomMember.md#onleft)
- [onMetadataUpdated](LocalRoomMember.md#onmetadataupdated)
- [onPublicationChanged](LocalRoomMember.md#onpublicationchanged)
- [onStreamPublished](LocalRoomMember.md#onstreampublished)
- [onStreamSubscribed](LocalRoomMember.md#onstreamsubscribed)
- [onStreamUnpublished](LocalRoomMember.md#onstreamunpublished)
- [onStreamUnsubscribed](LocalRoomMember.md#onstreamunsubscribed)
- [onSubscriptionChanged](LocalRoomMember.md#onsubscriptionchanged)
- [publications](LocalRoomMember.md#publications)
- [room](LocalRoomMember.md#room)
- [roomId](LocalRoomMember.md#roomid)
- [roomName](LocalRoomMember.md#roomname)
- [roomType](LocalRoomMember.md#roomtype)
- [side](LocalRoomMember.md#side)
- [status](LocalRoomMember.md#status)
- [subscriptions](LocalRoomMember.md#subscriptions)

### Methods

- [leave](LocalRoomMember.md#leave)
- [subscribe](LocalRoomMember.md#subscribe)
- [unpublish](LocalRoomMember.md#unpublish)
- [unsubscribe](LocalRoomMember.md#unsubscribe)
- [updateMetadata](LocalRoomMember.md#updatemetadata)

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

### onPublicationChanged

• **onPublicationChanged**: [`Event`](../classes/Event.md)<`void`\>

**`description`** {japanese} このMemberがStreamをSubscribeしたときに発火するイベント

___

### onStreamPublished

• **onStreamPublished**: [`Event`](../classes/Event.md)<{ `publication`: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このMemberがStreamをPublishしたときに発火するイベント

___

### onStreamSubscribed

• **onStreamSubscribed**: [`Event`](../classes/Event.md)<{ `stream`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このMemberがStreamをSubscribeしたときに発火するイベント

___

### onStreamUnpublished

• **onStreamUnpublished**: [`Event`](../classes/Event.md)<{ `publication`: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このMemberがStreamをUnPublishしたときに発火するイベント

___

### onStreamUnsubscribed

• **onStreamUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このMemberがStreamをUnsubscribeしたときに発火するイベント

___

### onSubscriptionChanged

• **onSubscriptionChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} Memberが Publish した Publication のリスト

#### Inherited from

[RoomMember](RoomMember.md).[publications](RoomMember.md#publications)

___

### room

• **room**: [`Room`](Room.md)

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

• **side**: ``"local"``

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

### leave

▸ **leave**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

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
