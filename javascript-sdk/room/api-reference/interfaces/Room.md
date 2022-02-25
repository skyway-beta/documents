[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / Room

# Interface: Room

## Hierarchy

- **`Room`**

  ↳ [`P2PRoom`](P2PRoom.md)

  ↳ [`SfuRoom`](SfuRoom.md)

## Table of contents

### Properties

- [disposed](Room.md#disposed)
- [id](Room.md#id)
- [members](Room.md#members)
- [metadata](Room.md#metadata)
- [name](Room.md#name)
- [onClosed](Room.md#onclosed)
- [onMemberJoined](Room.md#onmemberjoined)
- [onMemberLeft](Room.md#onmemberleft)
- [onMemberMetadataUpdated](Room.md#onmembermetadataupdated)
- [onMembershipChanged](Room.md#onmembershipchanged)
- [onMetadataUpdated](Room.md#onmetadataupdated)
- [onPublicationChanged](Room.md#onpublicationchanged)
- [onPublicationMetadataUpdated](Room.md#onpublicationmetadataupdated)
- [onStreamPublished](Room.md#onstreampublished)
- [onStreamSubscribed](Room.md#onstreamsubscribed)
- [onStreamUnpublished](Room.md#onstreamunpublished)
- [onStreamUnsubscribed](Room.md#onstreamunsubscribed)
- [onSubscriptionChangedEvent](Room.md#onsubscriptionchangedevent)
- [publications](Room.md#publications)
- [status](Room.md#status)
- [subscriptions](Room.md#subscriptions)
- [type](Room.md#type)

### Methods

- [close](Room.md#close)
- [dispose](Room.md#dispose)
- [join](Room.md#join)
- [leave](Room.md#leave)
- [memberMoveFromOtherRoom](Room.md#membermovefromotherroom)
- [updateMetadata](Room.md#updatemetadata)

## Properties

### disposed

• `Readonly` **disposed**: `boolean`

___

### id

• `Readonly` **id**: `string`

___

### members

• `Readonly` **members**: [`RemoteRoomMember`](RemoteRoomMember.md)[]

**`description`** {japanese} Roomに参加しているMemberのリスト

___

### metadata

• `Optional` `Readonly` **metadata**: `string`

___

### name

• `Optional` `Readonly` **name**: `string`

___

### onClosed

• `Readonly` **onClosed**: `Event`<[`RoomClosedEvent`](RoomClosedEvent.md)\>

___

### onMemberJoined

• `Readonly` **onMemberJoined**: `Event`<[`MemberJoinedEvent`](MemberJoinedEvent.md)\>

**`description`** {japanese} RoomにMemberが参加したときに発火するイベント

___

### onMemberLeft

• `Readonly` **onMemberLeft**: `Event`<[`MemberLeftEvent`](MemberLeftEvent.md)\>

**`description`** {japanese} RoomからMemberが離脱したときに発火するイベント

___

### onMemberMetadataUpdated

• `Readonly` **onMemberMetadataUpdated**: `Event`<[`MemberMetadataUpdatedEvent`](MemberMetadataUpdatedEvent.md)\>

**`description`** {japanese} Room上のMemberのメタデータが変更されたときに発火するイベント

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: `Event`<[`MembershipChangedEvent`](MembershipChangedEvent.md)\>

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<[`RoomMetadataUpdatedEvent`](RoomMetadataUpdatedEvent.md)\>

___

### onPublicationChanged

• `Readonly` **onPublicationChanged**: `Event`<[`PublicationChangedEvent`](PublicationChangedEvent.md)\>

___

### onPublicationMetadataUpdated

• `Readonly` **onPublicationMetadataUpdated**: `Event`<[`PublicationMetadataUpdatedEvent`](PublicationMetadataUpdatedEvent.md)\>

**`description`** {japanese} Room上のPublicationのメタデータが変更されたときに発火するイベント

___

### onStreamPublished

• `Readonly` **onStreamPublished**: `Event`<[`StreamPublishedEvent`](StreamPublishedEvent.md)\>

**`description`** {japanese} RoomにStreamがPublishされたときに発火するイベント

___

### onStreamSubscribed

• `Readonly` **onStreamSubscribed**: `Event`<[`StreamSubscribedEvent`](StreamSubscribedEvent.md)\>

**`description`** {japanese} Room上のStreamがSubscribeされたときに発火するイベント

___

### onStreamUnpublished

• `Readonly` **onStreamUnpublished**: `Event`<[`StreamUnpublishedEvent`](StreamUnpublishedEvent.md)\>

**`description`** {japanese} RoomからStreamがUnPublishされたときに発火するイベント

___

### onStreamUnsubscribed

• `Readonly` **onStreamUnsubscribed**: `Event`<[`StreamUnsubscribedEvent`](StreamUnsubscribedEvent.md)\>

**`description`** {japanese} Room上のStreamがUnSubscribeされたときに発火するイベント

___

### onSubscriptionChangedEvent

• `Readonly` **onSubscriptionChangedEvent**: `Event`<[`SubscriptionChangedEvent`](SubscriptionChangedEvent.md)\>

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} RoomにPublishされているStreamのPublicationのリスト

___

### status

• `Readonly` **status**: `ChannelStatus`

___

### subscriptions

• `Readonly` **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

**`description`** {japanese} Room上のStreamのSubscription情報のリスト

___

### type

• `Readonly` **type**: ``"sfu"`` \| ``"p2p"``

## Methods

### close

▸ **close**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

___

### dispose

▸ **dispose**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

___

### join

▸ **join**(`memberInit?`): `Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

**`description`** {japanese} RoomにMemberを参加させる

#### Parameters

| Name | Type |
| :------ | :------ |
| `memberInit?` | [`RoomMemberInit`](RoomMemberInit.md) |

#### Returns

`Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

___

### leave

▸ **leave**(`member`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`RoomMember`](RoomMember.md) |

#### Returns

`Promise`<`void`\>

___

### memberMoveFromOtherRoom

▸ **memberMoveFromOtherRoom**(`member`): `Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`LocalRoomMember`](LocalRoomMember.md) |

#### Returns

`Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

___

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>
