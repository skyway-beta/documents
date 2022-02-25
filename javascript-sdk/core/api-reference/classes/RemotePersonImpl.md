[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemotePersonImpl

# Class: RemotePersonImpl

## Hierarchy

- `MemberImpl`

  ↳ **`RemotePersonImpl`**

## Implements

- [`RemotePerson`](../modules.md#remoteperson)

## Table of contents

### Constructors

- [constructor](RemotePersonImpl.md#constructor)

### Properties

- [\_events](RemotePersonImpl.md#_events)
- [channel](RemotePersonImpl.md#channel)
- [id](RemotePersonImpl.md#id)
- [name](RemotePersonImpl.md#name)
- [onJoined](RemotePersonImpl.md#onjoined)
- [onLeft](RemotePersonImpl.md#onleft)
- [onMembershipChanged](RemotePersonImpl.md#onmembershipchanged)
- [onMetadataUpdated](RemotePersonImpl.md#onmetadataupdated)
- [onPublicationSubscribed](RemotePersonImpl.md#onpublicationsubscribed)
- [onPublicationUnsubscribed](RemotePersonImpl.md#onpublicationunsubscribed)
- [plugin](RemotePersonImpl.md#plugin)
- [side](RemotePersonImpl.md#side)
- [subtype](RemotePersonImpl.md#subtype)
- [type](RemotePersonImpl.md#type)

### Accessors

- [metadata](RemotePersonImpl.md#metadata)
- [publications](RemotePersonImpl.md#publications)
- [status](RemotePersonImpl.md#status)
- [subscriptions](RemotePersonImpl.md#subscriptions)

### Methods

- [subscribe](RemotePersonImpl.md#subscribe)
- [toJSON](RemotePersonImpl.md#tojson)
- [unsubscribe](RemotePersonImpl.md#unsubscribe)
- [updateMetadata](RemotePersonImpl.md#updatemetadata)

## Constructors

### constructor

• **new RemotePersonImpl**(`args`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `args` | `Object` |
| `args.channel` | [`SkyWayChannel`](SkyWayChannel.md) |
| `args.id` | `string` |
| `args.metadata?` | `string` |
| `args.name?` | `string` |
| `args.plugin` | `PersonPlugin` |

#### Overrides

MemberImpl.constructor

## Properties

### \_events

• `Readonly` **\_events**: `Events`

#### Implementation of

RemotePerson.\_events

#### Inherited from

MemberImpl.\_events

___

### channel

• `Readonly` **channel**: [`SkyWayChannel`](SkyWayChannel.md)

#### Implementation of

RemotePerson.channel

#### Inherited from

MemberImpl.channel

___

### id

• `Readonly` **id**: `string`

#### Implementation of

RemotePerson.id

#### Inherited from

MemberImpl.id

___

### name

• `Optional` `Readonly` **name**: `string`

#### Implementation of

RemotePerson.name

#### Inherited from

MemberImpl.name

___

### onJoined

• `Readonly` **onJoined**: [`Event`](Event.md)<`void`\>

#### Implementation of

RemotePerson.onJoined

#### Inherited from

MemberImpl.onJoined

___

### onLeft

• `Readonly` **onLeft**: [`Event`](Event.md)<`void`\>

#### Implementation of

RemotePerson.onLeft

#### Inherited from

MemberImpl.onLeft

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: [`Event`](Event.md)<`void`\>

#### Implementation of

RemotePerson.onMembershipChanged

#### Inherited from

MemberImpl.onMembershipChanged

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](Event.md)<`string`\>

#### Implementation of

RemotePerson.onMetadataUpdated

#### Inherited from

MemberImpl.onMetadataUpdated

___

### onPublicationSubscribed

• `Readonly` **onPublicationSubscribed**: [`Event`](Event.md)<{ `stream?`: [`RemoteStream`](../modules.md#remotestream) ; `subscription`: [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Implementation of

RemotePerson.onPublicationSubscribed

___

### onPublicationUnsubscribed

• `Readonly` **onPublicationUnsubscribed**: [`Event`](Event.md)<{ `subscription`: [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Implementation of

RemotePerson.onPublicationUnsubscribed

___

### plugin

• `Readonly` **plugin**: `PersonPlugin`

___

### side

• `Readonly` **side**: ``"remote"``

#### Implementation of

RemotePerson.side

#### Overrides

MemberImpl.side

___

### subtype

• `Readonly` **subtype**: ``"person"``

#### Implementation of

RemotePerson.subtype

#### Overrides

MemberImpl.subtype

___

### type

• `Readonly` **type**: ``"person"``

#### Implementation of

RemotePerson.type

#### Overrides

MemberImpl.type

## Accessors

### metadata

• `get` **metadata**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Implementation of

RemotePerson.metadata

#### Inherited from

MemberImpl.metadata

___

### publications

• `get` **publications**(): [`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Returns

[`Publication`](../interfaces/Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Implementation of

RemotePerson.publications

#### Inherited from

MemberImpl.publications

___

### status

• `get` **status**(): [`MemberStatus`](../modules.md#memberstatus)

#### Returns

[`MemberStatus`](../modules.md#memberstatus)

#### Implementation of

RemotePerson.status

#### Inherited from

MemberImpl.status

___

### subscriptions

• `get` **subscriptions**(): [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Returns

[`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Implementation of

RemotePerson.subscriptions

#### Inherited from

MemberImpl.subscriptions

## Methods

### subscribe

▸ **subscribe**(`publicationId`): `Promise`<{ `subscription`: [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<{ `subscription`: [`Subscription`](../interfaces/Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

#### Implementation of

RemotePerson.subscribe

___

### toJSON

▸ **toJSON**(): `Member`

#### Returns

`Member`

#### Implementation of

RemotePerson.toJSON

#### Inherited from

MemberImpl.toJSON

___

### unsubscribe

▸ **unsubscribe**(`subscriptionId`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Promise`<`void`\>

#### Implementation of

RemotePerson.unsubscribe

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

RemotePerson.updateMetadata

#### Inherited from

MemberImpl.updateMetadata
