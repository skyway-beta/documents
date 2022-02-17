[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Channel

# Interface: Channel

## Implemented by

- [`SkyWayChannel`](../classes/SkyWayChannel.md)

## Table of contents

### Properties

- [appId](Channel.md#appid)
- [bots](Channel.md#bots)
- [id](Channel.md#id)
- [members](Channel.md#members)
- [metadata](Channel.md#metadata)
- [name](Channel.md#name)
- [onClosed](Channel.md#onclosed)
- [onMemberJoined](Channel.md#onmemberjoined)
- [onMemberLeft](Channel.md#onmemberleft)
- [onMemberMetadataUpdated](Channel.md#onmembermetadataupdated)
- [onMembershipChanged](Channel.md#onmembershipchanged)
- [onMetadataUpdated](Channel.md#onmetadataupdated)
- [onPublicationChanged](Channel.md#onpublicationchanged)
- [onPublicationMetadataUpdated](Channel.md#onpublicationmetadataupdated)
- [onStreamPublished](Channel.md#onstreampublished)
- [onStreamSubscribed](Channel.md#onstreamsubscribed)
- [onStreamUnpublished](Channel.md#onstreamunpublished)
- [onStreamUnsubscribed](Channel.md#onstreamunsubscribed)
- [onSubscriptionChanged](Channel.md#onsubscriptionchanged)
- [persons](Channel.md#persons)
- [publications](Channel.md#publications)
- [status](Channel.md#status)
- [subscriptions](Channel.md#subscriptions)

### Methods

- [close](Channel.md#close)
- [dispose](Channel.md#dispose)
- [join](Channel.md#join)
- [leave](Channel.md#leave)
- [memberMoveFromOtherChannel](Channel.md#membermovefromotherchannel)
- [updateMetadata](Channel.md#updatemetadata)

## Properties

### appId

• **appId**: `string`

___

### bots

• **bots**: [`RemoteMember`](RemoteMember.md)[]

**`description`** {japanese} Channel中のBotの一覧を取得する

___

### id

• **id**: `string`

___

### members

• **members**: [`RemoteMember`](RemoteMember.md)[]

**`description`** {japanese} Channel中のMemberの一覧を取得する

___

### metadata

• `Optional` **metadata**: `string`

___

### name

• `Optional` **name**: `string`

___

### onClosed

• **onClosed**: [`Event`](../classes/Event.md)<[`ChannelClosedEvent`](ChannelClosedEvent.md)\>

**`description`** {japanese} このChannelが閉じられた時に発生するイベント

___

### onMemberJoined

• **onMemberJoined**: [`Event`](../classes/Event.md)<[`MemberJoinedEvent`](MemberJoinedEvent.md)\>

**`description`** {japanese} ChannelにMemberが参加した時に発生するイベント

___

### onMemberLeft

• **onMemberLeft**: [`Event`](../classes/Event.md)<[`MemberLeftEvent`](MemberLeftEvent.md)\>

**`description`** {japanese} ChannelからMemberが退出した時に発生するイベント

___

### onMemberMetadataUpdated

• **onMemberMetadataUpdated**: [`Event`](../classes/Event.md)<[`MemberMetadataUpdatedEvent`](MemberMetadataUpdatedEvent.md)\>

**`description`** {japanese} MemberのMetadataが更新された時に発生するイベント

___

### onMembershipChanged

• **onMembershipChanged**: [`Event`](../classes/Event.md)<[`MembershipChangedEvent`](MembershipChangedEvent.md)\>

___

### onMetadataUpdated

• **onMetadataUpdated**: [`Event`](../classes/Event.md)<[`ChannelMetadataUpdatedEvent`](ChannelMetadataUpdatedEvent.md)\>

**`description`** {japanese} このChannelのMetadataが更新された時に発生するイベント

___

### onPublicationChanged

• **onPublicationChanged**: [`Event`](../classes/Event.md)<[`PublicationChangedEvent`](PublicationChangedEvent.md)\>

___

### onPublicationMetadataUpdated

• **onPublicationMetadataUpdated**: [`Event`](../classes/Event.md)<[`PublicationMetadataUpdatedEvent`](PublicationMetadataUpdatedEvent.md)\>

**`description`** {japanese} StreamのPublicationのMetadataが更新された時に発生するイベント

___

### onStreamPublished

• **onStreamPublished**: [`Event`](../classes/Event.md)<[`StreamPublishedEvent`](StreamPublishedEvent.md)\>

**`description`** {japanese} ChannelのStreamがPublishされた時に発生するイベント

___

### onStreamSubscribed

• **onStreamSubscribed**: [`Event`](../classes/Event.md)<[`StreamSubscribedEvent`](StreamSubscribedEvent.md)\>

**`description`** {japanese} ChannelのPublicationがSubscribeされた時に発生するイベント

___

### onStreamUnpublished

• **onStreamUnpublished**: [`Event`](../classes/Event.md)<[`StreamUnpublishedEvent`](StreamUnpublishedEvent.md)\>

**`description`** {japanese} ChannelからStreamがUnpublishされた時に発生するイベント

___

### onStreamUnsubscribed

• **onStreamUnsubscribed**: [`Event`](../classes/Event.md)<[`StreamUnsubscribedEvent`](StreamUnsubscribedEvent.md)\>

**`description`** {japanese} ChannelのPublicationがUnsubscribeされた時に発生するイベント

___

### onSubscriptionChanged

• **onSubscriptionChanged**: [`Event`](../classes/Event.md)<[`SubscriptionChangedEvent`](SubscriptionChangedEvent.md)\>

___

### persons

• **persons**: [`LocalPerson`](LocalPerson.md)[]

**`description`** {japanese} Channel中のLocalPersonの一覧を取得する

___

### publications

• **publications**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

**`description`** {japanese} Channel中のPublicationの一覧を取得する

___

### status

• **status**: [`ChannelStatus`](../modules.md#channelstatus)

___

### subscriptions

• **subscriptions**: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

**`description`** {japanese} Channel中のSubscriptionの一覧を取得する

## Methods

### close

▸ **close**(): `Promise`<`void`\>

**`description`** {japanese} Channelを閉じる

#### Returns

`Promise`<`void`\>

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

___

### join

▸ **join**(`memberInit?`): `Promise`<[`LocalPerson`](LocalPerson.md)\>

**`description`** {japanese} ChannelにMemberを追加する

#### Parameters

| Name | Type |
| :------ | :------ |
| `memberInit?` | `Object` |
| `memberInit.keepaliveIntervalSec?` | `number` |
| `memberInit.metadata?` | `string` |
| `memberInit.name?` | `string` |

#### Returns

`Promise`<[`LocalPerson`](LocalPerson.md)\>

___

### leave

▸ **leave**(`member`): `Promise`<`void`\>

**`description`** {japanese} ChannelからMemberを退出させる

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`Member`](Member.md) |

#### Returns

`Promise`<`void`\>

___

### memberMoveFromOtherChannel

▸ **memberMoveFromOtherChannel**(`adapter`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `adapter` | [`LocalPerson`](LocalPerson.md) |

#### Returns

`Promise`<`void`\>

___

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

**`description`** {japanese} ChannelのMetadataを更新する

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>