[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / P2PRoom

# Interface: P2PRoom

## Hierarchy

- [`Room`](Room.md)

  ↳ **`P2PRoom`**

## Table of contents

### Properties

- [id](P2PRoom.md#id)
- [members](P2PRoom.md#members)
- [metadata](P2PRoom.md#metadata)
- [name](P2PRoom.md#name)
- [onClosed](P2PRoom.md#onclosed)
- [onMemberJoined](P2PRoom.md#onmemberjoined)
- [onMemberLeft](P2PRoom.md#onmemberleft)
- [onMemberMetadataUpdated](P2PRoom.md#onmembermetadataupdated)
- [onMembershipChanged](P2PRoom.md#onmembershipchanged)
- [onMetadataUpdated](P2PRoom.md#onmetadataupdated)
- [onPublicationChanged](P2PRoom.md#onpublicationchanged)
- [onPublicationMetadataUpdated](P2PRoom.md#onpublicationmetadataupdated)
- [onStreamPublished](P2PRoom.md#onstreampublished)
- [onStreamSubscribed](P2PRoom.md#onstreamsubscribed)
- [onStreamUnpublished](P2PRoom.md#onstreamunpublished)
- [onStreamUnsubscribed](P2PRoom.md#onstreamunsubscribed)
- [onSubscriptionChangedEvent](P2PRoom.md#onsubscriptionchangedevent)
- [publications](P2PRoom.md#publications)
- [status](P2PRoom.md#status)
- [subscriptions](P2PRoom.md#subscriptions)
- [type](P2PRoom.md#type)

### Methods

- [close](P2PRoom.md#close)
- [dispose](P2PRoom.md#dispose)
- [join](P2PRoom.md#join)
- [leave](P2PRoom.md#leave)
- [memberMoveFromOtherRoom](P2PRoom.md#membermovefromotherroom)
- [updateMetadata](P2PRoom.md#updatemetadata)

## Properties

### id

• `Readonly` **id**: `string`

#### Inherited from

[Room](Room.md).[id](Room.md#id)

___

### members

• `Readonly` **members**: [`RoomMember`](RoomMember.md)[]

**`description`** {japanese} Roomに参加しているMemberのリスト

#### Inherited from

[Room](Room.md).[members](Room.md#members)

___

### metadata

• `Optional` `Readonly` **metadata**: `string`

#### Inherited from

[Room](Room.md).[metadata](Room.md#metadata)

___

### name

• `Optional` `Readonly` **name**: `string`

#### Inherited from

[Room](Room.md).[name](Room.md#name)

___

### onClosed

• `Readonly` **onClosed**: `Event`<[`RoomClosedEvent`](RoomClosedEvent.md)\>

#### Inherited from

[Room](Room.md).[onClosed](Room.md#onclosed)

___

### onMemberJoined

• `Readonly` **onMemberJoined**: `Event`<[`MemberJoinedEvent`](MemberJoinedEvent.md)\>

**`description`** {japanese} RoomにMemberが参加したときに発火するイベント

#### Inherited from

[Room](Room.md).[onMemberJoined](Room.md#onmemberjoined)

___

### onMemberLeft

• `Readonly` **onMemberLeft**: `Event`<[`MemberLeftEvent`](MemberLeftEvent.md)\>

**`description`** {japanese} RoomからMemberが離脱したときに発火するイベント

#### Inherited from

[Room](Room.md).[onMemberLeft](Room.md#onmemberleft)

___

### onMemberMetadataUpdated

• `Readonly` **onMemberMetadataUpdated**: `Event`<[`MemberMetadataUpdatedEvent`](MemberMetadataUpdatedEvent.md)\>

**`description`** {japanese} Room上のMemberのメタデータが変更されたときに発火するイベント

#### Inherited from

[Room](Room.md).[onMemberMetadataUpdated](Room.md#onmembermetadataupdated)

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: `Event`<[`MembershipChangedEvent`](MembershipChangedEvent.md)\>

#### Inherited from

[Room](Room.md).[onMembershipChanged](Room.md#onmembershipchanged)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<[`RoomMetadataUpdatedEvent`](RoomMetadataUpdatedEvent.md)\>

#### Inherited from

[Room](Room.md).[onMetadataUpdated](Room.md#onmetadataupdated)

___

### onPublicationChanged

• `Readonly` **onPublicationChanged**: `Event`<[`PublicationChangedEvent`](PublicationChangedEvent.md)\>

#### Inherited from

[Room](Room.md).[onPublicationChanged](Room.md#onpublicationchanged)

___

### onPublicationMetadataUpdated

• `Readonly` **onPublicationMetadataUpdated**: `Event`<[`PublicationMetadataUpdatedEvent`](PublicationMetadataUpdatedEvent.md)\>

**`description`** {japanese} Room上のPublicationのメタデータが変更されたときに発火するイベント

#### Inherited from

[Room](Room.md).[onPublicationMetadataUpdated](Room.md#onpublicationmetadataupdated)

___

### onStreamPublished

• `Readonly` **onStreamPublished**: `Event`<[`StreamPublishedEvent`](StreamPublishedEvent.md)\>

**`description`** {japanese} RoomにStreamがPublishされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamPublished](Room.md#onstreampublished)

___

### onStreamSubscribed

• `Readonly` **onStreamSubscribed**: `Event`<[`StreamSubscribedEvent`](StreamSubscribedEvent.md)\>

**`description`** {japanese} Room上のStreamがSubscribeされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamSubscribed](Room.md#onstreamsubscribed)

___

### onStreamUnpublished

• `Readonly` **onStreamUnpublished**: `Event`<[`StreamUnpublishedEvent`](StreamUnpublishedEvent.md)\>

**`description`** {japanese} RoomからStreamがUnPublishされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamUnpublished](Room.md#onstreamunpublished)

___

### onStreamUnsubscribed

• `Readonly` **onStreamUnsubscribed**: `Event`<[`StreamUnsubscribedEvent`](StreamUnsubscribedEvent.md)\>

**`description`** {japanese} Room上のStreamがUnSubscribeされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamUnsubscribed](Room.md#onstreamunsubscribed)

___

### onSubscriptionChangedEvent

• `Readonly` **onSubscriptionChangedEvent**: `Event`<[`SubscriptionChangedEvent`](SubscriptionChangedEvent.md)\>

#### Inherited from

[Room](Room.md).[onSubscriptionChangedEvent](Room.md#onsubscriptionchangedevent)

___

### publications

• `Readonly` **publications**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} RoomにPublishされているStreamのPublicationのリスト

#### Inherited from

[Room](Room.md).[publications](Room.md#publications)

___

### status

• `Readonly` **status**: `ChannelStatus`

#### Inherited from

[Room](Room.md).[status](Room.md#status)

___

### subscriptions

• `Readonly` **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

**`description`** {japanese} Room上のStreamのSubscription情報のリスト

#### Inherited from

[Room](Room.md).[subscriptions](Room.md#subscriptions)

___

### type

• `Readonly` **type**: ``"sfu"`` \| ``"p2p"``

#### Inherited from

[Room](Room.md).[type](Room.md#type)

## Methods

### close

▸ **close**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

#### Inherited from

[Room](Room.md).[close](Room.md#close)

___

### dispose

▸ **dispose**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

#### Inherited from

[Room](Room.md).[dispose](Room.md#dispose)

___

### join

▸ **join**(`memberInit?`): `Promise`<[`LocalP2PRoomMember`](../classes/LocalP2PRoomMember.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `memberInit?` | `RoomMemberInit` |

#### Returns

`Promise`<[`LocalP2PRoomMember`](../classes/LocalP2PRoomMember.md)\>

#### Overrides

[Room](Room.md).[join](Room.md#join)

___

### leave

▸ **leave**(`member`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`RoomMember`](RoomMember.md) |

#### Returns

`Promise`<`void`\>

#### Inherited from

[Room](Room.md).[leave](Room.md#leave)

___

### memberMoveFromOtherRoom

▸ **memberMoveFromOtherRoom**(`member`): `Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`LocalRoomMember`](LocalRoomMember.md) |

#### Returns

`Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

#### Inherited from

[Room](Room.md).[memberMoveFromOtherRoom](Room.md#membermovefromotherroom)

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

[Room](Room.md).[updateMetadata](Room.md#updatemetadata)
