[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalRoomMember

# Interface: LocalRoomMember

## Hierarchy

- [`RoomMember`](RoomMember.md)

  ↳ **`LocalRoomMember`**

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
- [publish](LocalRoomMember.md#publish)
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

• `Readonly` **onLeft**: `Event`<`void`\>

#### Inherited from

[RoomMember](RoomMember.md).[onLeft](RoomMember.md#onleft)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<`string`\>

#### Inherited from

[RoomMember](RoomMember.md).[onMetadataUpdated](RoomMember.md#onmetadataupdated)

___

### onPublicationChanged

• **onPublicationChanged**: `Event`<`void`\>

**`description`** {japanese} このMemberがStreamをSubscribeしたときに発火するイベント

___

### onStreamPublished

• **onStreamPublished**: `Event`<{ `publication`: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このMemberがStreamをPublishしたときに発火するイベント

___

### onStreamSubscribed

• **onStreamSubscribed**: `Event`<{ `stream`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

___

### onStreamUnpublished

• **onStreamUnpublished**: `Event`<{ `publication`: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このMemberがStreamをUnPublishしたときに発火するイベント

___

### onStreamUnsubscribed

• **onStreamUnsubscribed**: `Event`<{ `subscription`: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このMemberがStreamをUnSubscribeしたときに発火するイベント

___

### onSubscriptionChanged

• **onSubscriptionChanged**: `Event`<`void`\>

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

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

#### Inherited from

[RoomMember](RoomMember.md).[subscriptions](RoomMember.md#subscriptions)

## Methods

### leave

▸ **leave**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

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

___

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
