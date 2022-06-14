[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemotePerson

# Interface: RemotePerson

## Hierarchy

- [`Person`](Person.md)

- [`RemotePersonInterface`](RemotePersonInterface.md)

  ↳ **`RemotePerson`**

## Table of contents

### Properties

- [channel](RemotePerson.md#channel)
- [id](RemotePerson.md#id)
- [metadata](RemotePerson.md#metadata)
- [name](RemotePerson.md#name)
- [onLeft](RemotePerson.md#onleft)
- [onMetadataUpdated](RemotePerson.md#onmetadataupdated)
- [onPublicationSubscribed](RemotePerson.md#onpublicationsubscribed)
- [onPublicationUnsubscribed](RemotePerson.md#onpublicationunsubscribed)
- [publications](RemotePerson.md#publications)
- [side](RemotePerson.md#side)
- [status](RemotePerson.md#status)
- [subscriptions](RemotePerson.md#subscriptions)
- [subtype](RemotePerson.md#subtype)
- [type](RemotePerson.md#type)

### Methods

- [subscribe](RemotePerson.md#subscribe)
- [unsubscribe](RemotePerson.md#unsubscribe)
- [updateMetadata](RemotePerson.md#updatemetadata)

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

### onPublicationSubscribed

• `Readonly` **onPublicationSubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemotePerson がPublicationをSubscribeしたとき

#### Inherited from

[RemotePersonInterface](RemotePersonInterface.md).[onPublicationSubscribed](RemotePersonInterface.md#onpublicationsubscribed)

___

### onPublicationUnsubscribed

• `Readonly` **onPublicationUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemotePerson がPublicationをUnsubscribeしたとき

#### Inherited from

[RemotePersonInterface](RemotePersonInterface.md).[onPublicationUnsubscribed](RemotePersonInterface.md#onpublicationunsubscribed)

___

### publications

• **publications**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

[Person](Person.md).[publications](Person.md#publications)

___

### side

• **side**: ``"remote"``

#### Overrides

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

### subscribe

▸ **subscribe**(`publicationId`): `Promise`<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemotePerson にPublicationをSubscribeさせる

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Inherited from

[RemotePersonInterface](RemotePersonInterface.md).[subscribe](RemotePersonInterface.md#subscribe)

___

### unsubscribe

▸ **unsubscribe**(`subscriptionId`): `Promise`<`void`\>

**`description`** {japanese} この RemotePerson にPublicationをUnsubscribeさせる

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

[RemotePersonInterface](RemotePersonInterface.md).[unsubscribe](RemotePersonInterface.md#unsubscribe)

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
