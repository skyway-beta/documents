[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalP2PRoomMember

# Class: LocalP2PRoomMember

## Hierarchy

- `LocalRoomMemberImpl`

  ↳ **`LocalP2PRoomMember`**

## Table of contents

### Constructors

- [constructor](LocalP2PRoomMember.md#constructor)

### Properties

- [\_local](LocalP2PRoomMember.md#_local)
- [onLeft](LocalP2PRoomMember.md#onleft)
- [onMetadataUpdated](LocalP2PRoomMember.md#onmetadataupdated)
- [onPublicationChanged](LocalP2PRoomMember.md#onpublicationchanged)
- [onStreamPublished](LocalP2PRoomMember.md#onstreampublished)
- [onStreamSubscribed](LocalP2PRoomMember.md#onstreamsubscribed)
- [onStreamUnpublished](LocalP2PRoomMember.md#onstreamunpublished)
- [onStreamUnsubscribed](LocalP2PRoomMember.md#onstreamunsubscribed)
- [onSubscriptionChanged](LocalP2PRoomMember.md#onsubscriptionchanged)
- [room](LocalP2PRoomMember.md#room)
- [side](LocalP2PRoomMember.md#side)

### Accessors

- [id](LocalP2PRoomMember.md#id)
- [metadata](LocalP2PRoomMember.md#metadata)
- [name](LocalP2PRoomMember.md#name)
- [publications](LocalP2PRoomMember.md#publications)
- [roomId](LocalP2PRoomMember.md#roomid)
- [roomName](LocalP2PRoomMember.md#roomname)
- [roomType](LocalP2PRoomMember.md#roomtype)
- [status](LocalP2PRoomMember.md#status)
- [subscriptions](LocalP2PRoomMember.md#subscriptions)

### Methods

- [\_listenRoomEvent](LocalP2PRoomMember.md#_listenroomevent)
- [\_updateRoom](LocalP2PRoomMember.md#_updateroom)
- [leave](LocalP2PRoomMember.md#leave)
- [publish](LocalP2PRoomMember.md#publish)
- [subscribe](LocalP2PRoomMember.md#subscribe)
- [unpublish](LocalP2PRoomMember.md#unpublish)
- [unsubscribe](LocalP2PRoomMember.md#unsubscribe)
- [updateMetadata](LocalP2PRoomMember.md#updatemetadata)

## Constructors

### constructor

• **new LocalP2PRoomMember**(`member`, `room`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | `LocalPersonAdapter` |
| `room` | `P2PRoomImpl` |

#### Overrides

LocalRoomMemberImpl.constructor

## Properties

### \_local

• `Readonly` **\_local**: `LocalPerson`

#### Inherited from

LocalRoomMemberImpl.\_local

___

### onLeft

• `Readonly` **onLeft**: `Event`<`void`\>

#### Inherited from

LocalRoomMemberImpl.onLeft

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<`string`\>

#### Inherited from

LocalRoomMemberImpl.onMetadataUpdated

___

### onPublicationChanged

• `Readonly` **onPublicationChanged**: `Event`<`void`\>

#### Inherited from

LocalRoomMemberImpl.onPublicationChanged

___

### onStreamPublished

• `Readonly` **onStreamPublished**: `Event`<{ `publication`: [`RoomPublication`](../interfaces/RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

#### Inherited from

LocalRoomMemberImpl.onStreamPublished

___

### onStreamSubscribed

• `Readonly` **onStreamSubscribed**: `Event`<{ `stream`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`RoomSubscription`](../interfaces/RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Inherited from

LocalRoomMemberImpl.onStreamSubscribed

___

### onStreamUnpublished

• `Readonly` **onStreamUnpublished**: `Event`<{ `publication`: [`RoomPublication`](../interfaces/RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

#### Inherited from

LocalRoomMemberImpl.onStreamUnpublished

___

### onStreamUnsubscribed

• `Readonly` **onStreamUnsubscribed**: `Event`<{ `subscription`: [`RoomSubscription`](../interfaces/RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Inherited from

LocalRoomMemberImpl.onStreamUnsubscribed

___

### onSubscriptionChanged

• `Readonly` **onSubscriptionChanged**: `Event`<`void`\>

#### Inherited from

LocalRoomMemberImpl.onSubscriptionChanged

___

### room

• **room**: `RoomImpl`

#### Inherited from

LocalRoomMemberImpl.room

___

### side

• `Readonly` **side**: ``"local"``

#### Inherited from

LocalRoomMemberImpl.side

## Accessors

### id

• `get` **id**(): `string`

#### Returns

`string`

#### Inherited from

LocalRoomMemberImpl.id

___

### metadata

• `get` **metadata**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Inherited from

LocalRoomMemberImpl.metadata

___

### name

• `get` **name**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Inherited from

LocalRoomMemberImpl.name

___

### publications

• `get` **publications**(): [`RoomPublication`](../interfaces/RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Returns

[`RoomPublication`](../interfaces/RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

LocalRoomMemberImpl.publications

___

### roomId

• `get` **roomId**(): `string`

#### Returns

`string`

#### Inherited from

LocalRoomMemberImpl.roomId

___

### roomName

• `get` **roomName**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Inherited from

LocalRoomMemberImpl.roomName

___

### roomType

• `get` **roomType**(): ``"sfu"`` \| ``"p2p"``

#### Returns

``"sfu"`` \| ``"p2p"``

#### Inherited from

LocalRoomMemberImpl.roomType

___

### status

• `get` **status**(): [`MemberStatus`](../modules.md#memberstatus)

#### Returns

[`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

LocalRoomMemberImpl.status

___

### subscriptions

• `get` **subscriptions**(): `RoomSubscriptionImpl`<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Returns

`RoomSubscriptionImpl`<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Inherited from

LocalRoomMemberImpl.subscriptions

## Methods

### \_listenRoomEvent

▸ `Protected` **_listenRoomEvent**(): `void`

#### Returns

`void`

#### Inherited from

LocalRoomMemberImpl.\_listenRoomEvent

___

### \_updateRoom

▸ **_updateRoom**(`room`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `room` | `P2PRoomImpl` |

#### Returns

`void`

#### Overrides

LocalRoomMemberImpl.\_updateRoom

___

### leave

▸ **leave**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

#### Inherited from

LocalRoomMemberImpl.leave

___

### publish

▸ **publish**(`stream`, `options?`): `Promise`<[`RoomPublication`](../interfaces/RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>\>

**`description`** {japanese} RoomにStreamをPublishする

#### Parameters

| Name | Type |
| :------ | :------ |
| `stream` | [`LocalStream`](../modules.md#localstream) |
| `options` | `PublicationOptions` |

#### Returns

`Promise`<[`RoomPublication`](../interfaces/RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>\>

#### Overrides

LocalRoomMemberImpl.publish

___

### subscribe

▸ **subscribe**<`T`\>(`publicationId`): `Promise`<{ `stream`: `T` ; `subscription`: [`RoomSubscription`](../interfaces/RoomSubscription.md)<`T`\>  }\>

**`description`** {japanese} MemberがRoom上のStreamのPublicationをSubscribeする

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`RemoteStream`](../modules.md#remotestream) = [`RemoteStream`](../modules.md#remotestream) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<{ `stream`: `T` ; `subscription`: [`RoomSubscription`](../interfaces/RoomSubscription.md)<`T`\>  }\>

#### Overrides

LocalRoomMemberImpl.subscribe

___

### unpublish

▸ **unpublish**(`publicationId`): `Promise`<`void`\>

**`description`** {japanese} Room上のStreamをUnPublishする

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<`void`\>

#### Overrides

LocalRoomMemberImpl.unpublish

___

### unsubscribe

▸ **unsubscribe**(`subscriptionId`): `Promise`<`void`\>

**`description`** {japanese} MemberがSubscribeしているStreamのSubscriptionをUnSubscribeする

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Promise`<`void`\>

#### Overrides

LocalRoomMemberImpl.unsubscribe

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

LocalRoomMemberImpl.updateMetadata
