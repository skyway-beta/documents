[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / SfuRoom

# Interface: SfuRoom

## Hierarchy

- [`Room`](Room.md)

  ↳ **`SfuRoom`**

## Table of contents

### Properties

- [disposed](SfuRoom.md#disposed)
- [id](SfuRoom.md#id)
- [members](SfuRoom.md#members)
- [metadata](SfuRoom.md#metadata)
- [name](SfuRoom.md#name)
- [onClosed](SfuRoom.md#onclosed)
- [onMemberJoined](SfuRoom.md#onmemberjoined)
- [onMemberLeft](SfuRoom.md#onmemberleft)
- [onMemberMetadataUpdated](SfuRoom.md#onmembermetadataupdated)
- [onMembershipChanged](SfuRoom.md#onmembershipchanged)
- [onMetadataUpdated](SfuRoom.md#onmetadataupdated)
- [onPublicationChanged](SfuRoom.md#onpublicationchanged)
- [onPublicationMetadataUpdated](SfuRoom.md#onpublicationmetadataupdated)
- [onStreamPublished](SfuRoom.md#onstreampublished)
- [onStreamSubscribed](SfuRoom.md#onstreamsubscribed)
- [onStreamUnpublished](SfuRoom.md#onstreamunpublished)
- [onStreamUnsubscribed](SfuRoom.md#onstreamunsubscribed)
- [onSubscriptionChangedEvent](SfuRoom.md#onsubscriptionchangedevent)
- [publications](SfuRoom.md#publications)
- [status](SfuRoom.md#status)
- [subscriptions](SfuRoom.md#subscriptions)
- [type](SfuRoom.md#type)

### Methods

- [close](SfuRoom.md#close)
- [dispose](SfuRoom.md#dispose)
- [join](SfuRoom.md#join)
- [leave](SfuRoom.md#leave)
- [moveRoom](SfuRoom.md#moveroom)
- [updateMetadata](SfuRoom.md#updatemetadata)

## Properties

### disposed

• `Readonly` **disposed**: `boolean`

#### Inherited from

[Room](Room.md).[disposed](Room.md#disposed)

___

### id

• `Readonly` **id**: `string`

#### Inherited from

[Room](Room.md).[id](Room.md#id)

___

### members

• `Readonly` **members**: [`RemoteRoomMember`](RemoteRoomMember.md)[]

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

• `Readonly` **onClosed**: [`Event`](../classes/Event.md)<[`RoomClosedEvent`](RoomClosedEvent.md)\>

#### Inherited from

[Room](Room.md).[onClosed](Room.md#onclosed)

___

### onMemberJoined

• `Readonly` **onMemberJoined**: [`Event`](../classes/Event.md)<[`MemberJoinedEvent`](MemberJoinedEvent.md)\>

**`description`** {japanese} RoomにMemberが参加したときに発火するイベント

#### Inherited from

[Room](Room.md).[onMemberJoined](Room.md#onmemberjoined)

___

### onMemberLeft

• `Readonly` **onMemberLeft**: [`Event`](../classes/Event.md)<[`MemberLeftEvent`](MemberLeftEvent.md)\>

**`description`** {japanese} RoomからMemberが離脱したときに発火するイベント

#### Inherited from

[Room](Room.md).[onMemberLeft](Room.md#onmemberleft)

___

### onMemberMetadataUpdated

• `Readonly` **onMemberMetadataUpdated**: [`Event`](../classes/Event.md)<[`MemberMetadataUpdatedEvent`](MemberMetadataUpdatedEvent.md)\>

**`description`** {japanese} Room上のMemberのメタデータが変更されたときに発火するイベント

#### Inherited from

[Room](Room.md).[onMemberMetadataUpdated](Room.md#onmembermetadataupdated)

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: [`Event`](../classes/Event.md)<[`MembershipChangedEvent`](MembershipChangedEvent.md)\>

#### Inherited from

[Room](Room.md).[onMembershipChanged](Room.md#onmembershipchanged)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](../classes/Event.md)<[`RoomMetadataUpdatedEvent`](RoomMetadataUpdatedEvent.md)\>

#### Inherited from

[Room](Room.md).[onMetadataUpdated](Room.md#onmetadataupdated)

___

### onPublicationChanged

• `Readonly` **onPublicationChanged**: [`Event`](../classes/Event.md)<[`PublicationChangedEvent`](PublicationChangedEvent.md)\>

#### Inherited from

[Room](Room.md).[onPublicationChanged](Room.md#onpublicationchanged)

___

### onPublicationMetadataUpdated

• `Readonly` **onPublicationMetadataUpdated**: [`Event`](../classes/Event.md)<[`PublicationMetadataUpdatedEvent`](PublicationMetadataUpdatedEvent.md)\>

**`description`** {japanese} Room上のPublicationのメタデータが変更されたときに発火するイベント

#### Inherited from

[Room](Room.md).[onPublicationMetadataUpdated](Room.md#onpublicationmetadataupdated)

___

### onStreamPublished

• `Readonly` **onStreamPublished**: [`Event`](../classes/Event.md)<[`StreamPublishedEvent`](StreamPublishedEvent.md)\>

**`description`** {japanese} RoomにStreamがPublishされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamPublished](Room.md#onstreampublished)

___

### onStreamSubscribed

• `Readonly` **onStreamSubscribed**: [`Event`](../classes/Event.md)<[`StreamSubscribedEvent`](StreamSubscribedEvent.md)\>

**`description`** {japanese} Room上のStreamがSubscribeされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamSubscribed](Room.md#onstreamsubscribed)

___

### onStreamUnpublished

• `Readonly` **onStreamUnpublished**: [`Event`](../classes/Event.md)<[`StreamUnpublishedEvent`](StreamUnpublishedEvent.md)\>

**`description`** {japanese} RoomからStreamがUnPublishされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamUnpublished](Room.md#onstreamunpublished)

___

### onStreamUnsubscribed

• `Readonly` **onStreamUnsubscribed**: [`Event`](../classes/Event.md)<[`StreamUnsubscribedEvent`](StreamUnsubscribedEvent.md)\>

**`description`** {japanese} Room上のStreamがUnSubscribeされたときに発火するイベント

#### Inherited from

[Room](Room.md).[onStreamUnsubscribed](Room.md#onstreamunsubscribed)

___

### onSubscriptionChangedEvent

• `Readonly` **onSubscriptionChangedEvent**: [`Event`](../classes/Event.md)<[`SubscriptionChangedEvent`](SubscriptionChangedEvent.md)\>

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

• `Readonly` **status**: [`ChannelStatus`](../modules.md#channelstatus)

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

▸ **join**(`memberInit?`): `Promise`<[`LocalSFURoomMember`](LocalSFURoomMember.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `memberInit?` | [`RoomMemberInit`](RoomMemberInit.md) |

#### Returns

`Promise`<[`LocalSFURoomMember`](LocalSFURoomMember.md)\>

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

### moveRoom

▸ **moveRoom**(`member`): `Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

**`description`** {japanese} 別のRoomのMemberを移動させる

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`LocalRoomMember`](LocalRoomMember.md) |

#### Returns

`Promise`<[`LocalRoomMember`](LocalRoomMember.md)\>

#### Inherited from

[Room](Room.md).[moveRoom](Room.md#moveroom)

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
