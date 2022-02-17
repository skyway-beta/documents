[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayChannel

# Class: SkyWayChannel

## Implements

- [`Channel`](../interfaces/Channel.md)

## Table of contents

### Constructors

- [constructor](SkyWayChannel.md#constructor)

### Properties

- [appId](SkyWayChannel.md#appid)
- [id](SkyWayChannel.md#id)
- [name](SkyWayChannel.md#name)
- [onClosed](SkyWayChannel.md#onclosed)
- [onMemberJoined](SkyWayChannel.md#onmemberjoined)
- [onMemberLeft](SkyWayChannel.md#onmemberleft)
- [onMemberMetadataUpdated](SkyWayChannel.md#onmembermetadataupdated)
- [onMembershipChanged](SkyWayChannel.md#onmembershipchanged)
- [onMetadataUpdated](SkyWayChannel.md#onmetadataupdated)
- [onPublicationChanged](SkyWayChannel.md#onpublicationchanged)
- [onPublicationMetadataUpdated](SkyWayChannel.md#onpublicationmetadataupdated)
- [onStreamPublished](SkyWayChannel.md#onstreampublished)
- [onStreamSubscribed](SkyWayChannel.md#onstreamsubscribed)
- [onStreamUnpublished](SkyWayChannel.md#onstreamunpublished)
- [onStreamUnsubscribed](SkyWayChannel.md#onstreamunsubscribed)
- [onSubscriptionChanged](SkyWayChannel.md#onsubscriptionchanged)

### Accessors

- [bots](SkyWayChannel.md#bots)
- [members](SkyWayChannel.md#members)
- [metadata](SkyWayChannel.md#metadata)
- [persons](SkyWayChannel.md#persons)
- [publications](SkyWayChannel.md#publications)
- [status](SkyWayChannel.md#status)
- [subscriptions](SkyWayChannel.md#subscriptions)

### Methods

- [close](SkyWayChannel.md#close)
- [dispose](SkyWayChannel.md#dispose)
- [join](SkyWayChannel.md#join)
- [leave](SkyWayChannel.md#leave)
- [memberMoveFromOtherChannel](SkyWayChannel.md#membermovefromotherchannel)
- [updateMetadata](SkyWayChannel.md#updatemetadata)
- [Create](SkyWayChannel.md#create)
- [Find](SkyWayChannel.md#find)
- [FindOrCreate](SkyWayChannel.md#findorcreate)

## Constructors

### constructor

• **new SkyWayChannel**(`_context`, `_channelImpl`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_context` | [`SkyWayContext`](SkyWayContext.md) |
| `_channelImpl` | `ChannelImpl` |

## Properties

### appId

• `Readonly` **appId**: `string`

#### Implementation of

[Channel](../interfaces/Channel.md).[appId](../interfaces/Channel.md#appid)

___

### id

• `Readonly` **id**: `string`

#### Implementation of

[Channel](../interfaces/Channel.md).[id](../interfaces/Channel.md#id)

___

### name

• `Readonly` **name**: `string`

#### Implementation of

[Channel](../interfaces/Channel.md).[name](../interfaces/Channel.md#name)

___

### onClosed

• `Readonly` **onClosed**: [`Event`](Event.md)<[`ChannelClosedEvent`](../interfaces/ChannelClosedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onClosed](../interfaces/Channel.md#onclosed)

___

### onMemberJoined

• `Readonly` **onMemberJoined**: [`Event`](Event.md)<[`MemberJoinedEvent`](../interfaces/MemberJoinedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onMemberJoined](../interfaces/Channel.md#onmemberjoined)

___

### onMemberLeft

• `Readonly` **onMemberLeft**: [`Event`](Event.md)<[`MemberLeftEvent`](../interfaces/MemberLeftEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onMemberLeft](../interfaces/Channel.md#onmemberleft)

___

### onMemberMetadataUpdated

• `Readonly` **onMemberMetadataUpdated**: [`Event`](Event.md)<[`MemberMetadataUpdatedEvent`](../interfaces/MemberMetadataUpdatedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onMemberMetadataUpdated](../interfaces/Channel.md#onmembermetadataupdated)

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: [`Event`](Event.md)<[`MembershipChangedEvent`](../interfaces/MembershipChangedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onMembershipChanged](../interfaces/Channel.md#onmembershipchanged)

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](Event.md)<[`ChannelMetadataUpdatedEvent`](../interfaces/ChannelMetadataUpdatedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onMetadataUpdated](../interfaces/Channel.md#onmetadataupdated)

___

### onPublicationChanged

• `Readonly` **onPublicationChanged**: [`Event`](Event.md)<[`PublicationChangedEvent`](../interfaces/PublicationChangedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onPublicationChanged](../interfaces/Channel.md#onpublicationchanged)

___

### onPublicationMetadataUpdated

• `Readonly` **onPublicationMetadataUpdated**: [`Event`](Event.md)<[`PublicationMetadataUpdatedEvent`](../interfaces/PublicationMetadataUpdatedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onPublicationMetadataUpdated](../interfaces/Channel.md#onpublicationmetadataupdated)

___

### onStreamPublished

• `Readonly` **onStreamPublished**: [`Event`](Event.md)<[`StreamPublishedEvent`](../interfaces/StreamPublishedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onStreamPublished](../interfaces/Channel.md#onstreampublished)

___

### onStreamSubscribed

• `Readonly` **onStreamSubscribed**: [`Event`](Event.md)<[`StreamSubscribedEvent`](../interfaces/StreamSubscribedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onStreamSubscribed](../interfaces/Channel.md#onstreamsubscribed)

___

### onStreamUnpublished

• `Readonly` **onStreamUnpublished**: [`Event`](Event.md)<[`StreamUnpublishedEvent`](../interfaces/StreamUnpublishedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onStreamUnpublished](../interfaces/Channel.md#onstreamunpublished)

___

### onStreamUnsubscribed

• `Readonly` **onStreamUnsubscribed**: [`Event`](Event.md)<[`StreamUnsubscribedEvent`](../interfaces/StreamUnsubscribedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onStreamUnsubscribed](../interfaces/Channel.md#onstreamunsubscribed)

___

### onSubscriptionChanged

• `Readonly` **onSubscriptionChanged**: [`Event`](Event.md)<[`SubscriptionChangedEvent`](../interfaces/SubscriptionChangedEvent.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[onSubscriptionChanged](../interfaces/Channel.md#onsubscriptionchanged)

## Accessors

### bots

• `get` **bots**(): [`RemoteMember`](../interfaces/RemoteMember.md)[]

#### Returns

[`RemoteMember`](../interfaces/RemoteMember.md)[]

#### Implementation of

[Channel](../interfaces/Channel.md).[bots](../interfaces/Channel.md#bots)

___

### members

• `get` **members**(): [`RemoteMember`](../interfaces/RemoteMember.md)[]

#### Returns

[`RemoteMember`](../interfaces/RemoteMember.md)[]

#### Implementation of

[Channel](../interfaces/Channel.md).[members](../interfaces/Channel.md#members)

___

### metadata

• `get` **metadata**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Implementation of

[Channel](../interfaces/Channel.md).[metadata](../interfaces/Channel.md#metadata)

___

### persons

• `get` **persons**(): [`LocalPerson`](../interfaces/LocalPerson.md)[]

#### Returns

[`LocalPerson`](../interfaces/LocalPerson.md)[]

#### Implementation of

[Channel](../interfaces/Channel.md).[persons](../interfaces/Channel.md#persons)

___

### publications

• `get` **publications**(): [`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Returns

[`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Implementation of

[Channel](../interfaces/Channel.md).[publications](../interfaces/Channel.md#publications)

___

### status

• `get` **status**(): [`ChannelStatus`](../modules.md#channelstatus)

#### Returns

[`ChannelStatus`](../modules.md#channelstatus)

#### Implementation of

[Channel](../interfaces/Channel.md).[status](../interfaces/Channel.md#status)

___

### subscriptions

• `get` **subscriptions**(): [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Returns

[`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Implementation of

[Channel](../interfaces/Channel.md).[subscriptions](../interfaces/Channel.md#subscriptions)

## Methods

### close

▸ **close**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

#### Implementation of

[Channel](../interfaces/Channel.md).[close](../interfaces/Channel.md#close)

___

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

#### Implementation of

[Channel](../interfaces/Channel.md).[dispose](../interfaces/Channel.md#dispose)

___

### join

▸ **join**(`options?`): `Promise`<[`LocalPerson`](../interfaces/LocalPerson.md)\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Object` |
| `options.keepaliveIntervalSec?` | ``null`` \| `number` |
| `options.metadata?` | `string` |
| `options.name?` | `string` |

#### Returns

`Promise`<[`LocalPerson`](../interfaces/LocalPerson.md)\>

#### Implementation of

[Channel](../interfaces/Channel.md).[join](../interfaces/Channel.md#join)

___

### leave

▸ **leave**(`member`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | [`Member`](../interfaces/Member.md) |

#### Returns

`Promise`<`void`\>

#### Implementation of

[Channel](../interfaces/Channel.md).[leave](../interfaces/Channel.md#leave)

___

### memberMoveFromOtherChannel

▸ **memberMoveFromOtherChannel**(`adapter`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `adapter` | [`LocalPerson`](../interfaces/LocalPerson.md) |

#### Returns

`Promise`<`void`\>

#### Implementation of

[Channel](../interfaces/Channel.md).[memberMoveFromOtherChannel](../interfaces/Channel.md#membermovefromotherchannel)

___

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>

#### Implementation of

[Channel](../interfaces/Channel.md).[updateMetadata](../interfaces/Channel.md#updatemetadata)

___

### Create

▸ `Static` **Create**(`context`, `init?`): `Promise`<[`Channel`](../interfaces/Channel.md)\>

**`description`** {japanese} Channelの作成

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `init` | [`ChannelInit`](../interfaces/ChannelInit.md) |

#### Returns

`Promise`<[`Channel`](../interfaces/Channel.md)\>

___

### Find

▸ `Static` **Find**(`context`, `query`): `Promise`<[`Channel`](../interfaces/Channel.md)\>

**`description`** {japanese} 既存のChannelの取得

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `query` | [`ChannelQuery`](../interfaces/ChannelQuery.md) |

#### Returns

`Promise`<[`Channel`](../interfaces/Channel.md)\>

___

### FindOrCreate

▸ `Static` **FindOrCreate**(`context`, `query`): `Promise`<[`Channel`](../interfaces/Channel.md)\>

**`description`** {japanese} Channelの取得を試み、存在しなければ作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `query` | [`ChannelInit`](../interfaces/ChannelInit.md) |

#### Returns

`Promise`<[`Channel`](../interfaces/Channel.md)\>
