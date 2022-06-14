[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / LocalPerson

# Interface: LocalPerson

## Hierarchy

- [`Person`](Person.md)

  ↳ **`LocalPerson`**

## Table of contents

### Properties

- [channel](LocalPerson.md#channel)
- [id](LocalPerson.md#id)
- [keepaliveIntervalSec](LocalPerson.md#keepaliveintervalsec)
- [metadata](LocalPerson.md#metadata)
- [name](LocalPerson.md#name)
- [onLeft](LocalPerson.md#onleft)
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

- [leave](LocalPerson.md#leave)
- [publish](LocalPerson.md#publish)
- [subscribe](LocalPerson.md#subscribe)
- [unpublish](LocalPerson.md#unpublish)
- [unsubscribe](LocalPerson.md#unsubscribe)
- [updateMetadata](LocalPerson.md#updatemetadata)

## Properties

### channel

• **channel**: [`Channel`](Channel.md)

#### Inherited from

[Person](Person.md).[channel](Person.md#channel)

___

### id

• **id**: `string`

#### Inherited from

[Person](Person.md).[id](Person.md#id)

___

### keepaliveIntervalSec

• `Optional` `Readonly` **keepaliveIntervalSec**: ``null`` \| `number`

___

### metadata

• `Optional` **metadata**: `string`

#### Inherited from

[Person](Person.md).[metadata](Person.md#metadata)

___

### name

• `Optional` **name**: `string`

#### Inherited from

[Person](Person.md).[name](Person.md#name)

___

### onLeft

• **onLeft**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

[Person](Person.md).[onLeft](Person.md#onleft)

___

### onMetadataUpdated

• **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

#### Inherited from

[Person](Person.md).[onMetadataUpdated](Person.md#onmetadataupdated)

___

### onPublicationChanged

• `Readonly` **onPublicationChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### onStreamPublished

• `Readonly` **onStreamPublished**: [`Event`](../classes/Event.md)<{ `publication`: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このPersonがStreamをPublishしたときに発火するイベント

___

### onStreamSubscribed

• `Readonly` **onStreamSubscribed**: [`Event`](../classes/Event.md)<{ `stream`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このPersonがStreamをSubscribeしたときに発火するイベント

___

### onStreamUnpublished

• `Readonly` **onStreamUnpublished**: [`Event`](../classes/Event.md)<{ `publication`: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>  }\>

**`description`** {japanese} このPersonがStreamをUnpublishしたときに発火するイベント

___

### onStreamUnsubscribed

• `Readonly` **onStreamUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} このPersonがStreamをUnsubscribeしたときに発火するイベント

___

### onSubscriptionChanged

• `Readonly` **onSubscriptionChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### publications

• **publications**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

[Person](Person.md).[publications](Person.md#publications)

___

### side

• **side**: [`MemberSide`](../modules.md#memberside)

#### Inherited from

[Person](Person.md).[side](Person.md#side)

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

[Person](Person.md).[status](Person.md#status)

___

### subscriptions

• **subscriptions**: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Inherited from

[Person](Person.md).[subscriptions](Person.md#subscriptions)

___

### subtype

• `Readonly` **subtype**: ``"person"``

#### Inherited from

[Person](Person.md).[subtype](Person.md#subtype)

___

### type

• `Readonly` **type**: ``"person"``

#### Inherited from

[Person](Person.md).[type](Person.md#type)

## Methods

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

▸ **subscribe**<`T`\>(`publication`): `Promise`<{ `stream`: `T` ; `subscription`: [`Subscription`](Subscription.md)<`T`\>  }\>

**`description`** {japanese} StreamのPublicationをSubscribeする

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`RemoteStream`](../modules.md#remotestream) = [`RemoteStream`](../modules.md#remotestream) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `string` \| [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\> |

#### Returns

`Promise`<{ `stream`: `T` ; `subscription`: [`Subscription`](Subscription.md)<`T`\>  }\>

___

### unpublish

▸ **unpublish**(`publication`): `Promise`<`void`\>

**`description`** {japanese} StreamのPublicationをUnpublishする

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `string` \| [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\> |

#### Returns

`Promise`<`void`\>

___

### unsubscribe

▸ **unsubscribe**(`subscription`): `Promise`<`void`\>

**`description`** {japanese} StreamのSubscriptionをUnsubscribeする

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscription` | `string` \| [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\> |

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

[Person](Person.md).[updateMetadata](Person.md#updatemetadata)
