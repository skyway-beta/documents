[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / LocalPerson

# Interface: LocalPerson

## Hierarchy

- `Person`

  ↳ **`LocalPerson`**

## Table of contents

### Properties

- [channel](LocalPerson.md#channel)
- [id](LocalPerson.md#id)
- [keepaliveIntervalSec](LocalPerson.md#keepaliveintervalsec)
- [metadata](LocalPerson.md#metadata)
- [name](LocalPerson.md#name)
- [onJoined](LocalPerson.md#onjoined)
- [onLeft](LocalPerson.md#onleft)
- [onMembershipChanged](LocalPerson.md#onmembershipchanged)
- [onMetadataUpdated](LocalPerson.md#onmetadataupdated)
- [onPublicationChanged](LocalPerson.md#onpublicationchanged)
- [onStreamPublished](LocalPerson.md#onstreampublished)
- [onStreamSubscribed](LocalPerson.md#onstreamsubscribed)
- [onStreamUnpublished](LocalPerson.md#onstreamunpublished)
- [onStreamUnsubscribed](LocalPerson.md#onstreamunsubscribed)
- [onSubscriptionChanged](LocalPerson.md#onsubscriptionchanged)
- [publications](LocalPerson.md#publications)
- [side](LocalPerson.md#side)
- [status](LocalPerson.md#status)
- [subscriptions](LocalPerson.md#subscriptions)
- [subtype](LocalPerson.md#subtype)
- [type](LocalPerson.md#type)

### Methods

- [getConnections](LocalPerson.md#getconnections)
- [leave](LocalPerson.md#leave)
- [publish](LocalPerson.md#publish)
- [subscribe](LocalPerson.md#subscribe)
- [unpublish](LocalPerson.md#unpublish)
- [unsubscribe](LocalPerson.md#unsubscribe)
- [updateMetadata](LocalPerson.md#updatemetadata)

## Properties

### channel

• **channel**: `SkyWayChannelImpl`

#### Inherited from

Person.channel

___

### id

• **id**: `string`

#### Inherited from

Person.id

___

### keepaliveIntervalSec

• `Optional` `Readonly` **keepaliveIntervalSec**: ``null`` \| `number`

___

### metadata

• `Optional` **metadata**: `string`

#### Inherited from

Person.metadata

___

### name

• `Optional` **name**: `string`

#### Inherited from

Person.name

___

### onJoined

• **onJoined**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

Person.onJoined

___

### onLeft

• **onLeft**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

Person.onLeft

___

### onMembershipChanged

• **onMembershipChanged**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

Person.onMembershipChanged

___

### onMetadataUpdated

• **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

#### Inherited from

Person.onMetadataUpdated

___

### onPublicationChanged

• **onPublicationChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### onStreamPublished

• **onStreamPublished**: [`Event`](../classes/Event.md)<{ `publication`: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このPersonがStreamをPublishしたときに発火するイベント

___

### onStreamSubscribed

• **onStreamSubscribed**: [`Event`](../classes/Event.md)<{ `stream`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このPersonがStreamをSubscribeしたときに発火するイベント

___

### onStreamUnpublished

• **onStreamUnpublished**: [`Event`](../classes/Event.md)<{ `publication`: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このPersonがStreamをUnpublishしたときに発火するイベント

___

### onStreamUnsubscribed

• **onStreamUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このPersonがStreamをUnsubscribeしたときに発火するイベント

___

### onSubscriptionChanged

• **onSubscriptionChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### publications

• **publications**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

Person.publications

___

### side

• **side**: [`MemberSide`](../modules.md#memberside)

#### Inherited from

Person.side

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

Person.status

___

### subscriptions

• **subscriptions**: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Inherited from

Person.subscriptions

___

### subtype

• `Readonly` **subtype**: ``"person"``

#### Inherited from

Person.subtype

___

### type

• `Readonly` **type**: ``"person"``

#### Inherited from

Person.type

## Methods

### getConnections

▸ **getConnections**(): [`SkyWayConnection`](SkyWayConnection.md)[]

#### Returns

[`SkyWayConnection`](SkyWayConnection.md)[]

___

### leave

▸ **leave**(): `Promise`<`void`\>

#### Returns

`Promise`<`void`\>

___

### publish

▸ **publish**<`T`\>(`stream`, `options?`): `Promise`<[`Publication`](Publication.md)<`T`\>\>

**`description`** {japanese} StreamをPublishする

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`LocalStream`](../modules.md#localstream) = [`LocalStream`](../modules.md#localstream) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `stream` | `T` |
| `options?` | [`PublicationOptions`](PublicationOptions.md) |

#### Returns

`Promise`<[`Publication`](Publication.md)<`T`\>\>

___

### subscribe

▸ **subscribe**<`T`\>(`publicationId`): `Promise`<{ `stream`: `T` ; `subscription`: [`Subscription`](Subscription.md)<`T`\>  }\>

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

`Promise`<{ `stream`: `T` ; `subscription`: [`Subscription`](Subscription.md)<`T`\>  }\>

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

**`description`** {japanese} metadataを更新する

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

Person.updateMetadata
