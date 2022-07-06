[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Person

# Interface: Person

## Hierarchy

- [`Member`](Member.md)

  ↳ **`Person`**

  ↳↳ [`LocalPerson`](LocalPerson.md)

## Table of contents

### Properties

- [channel](Person.md#channel)
- [id](Person.md#id)
- [metadata](Person.md#metadata)
- [name](Person.md#name)
- [onLeft](Person.md#onleft)
- [onMetadataUpdated](Person.md#onmetadataupdated)
- [publications](Person.md#publications)
- [side](Person.md#side)
- [status](Person.md#status)
- [subscriptions](Person.md#subscriptions)
- [subtype](Person.md#subtype)
- [type](Person.md#type)

### Methods

- [updateMetadata](Person.md#updatemetadata)

## Properties

### channel

• **channel**: [`Channel`](Channel.md)

#### Inherited from

[Member](Member.md).[channel](Member.md#channel)

___

### id

• **id**: `string`

#### Inherited from

[Member](Member.md).[id](Member.md#id)

___

### metadata

• `Optional` **metadata**: `string`

#### Inherited from

[Member](Member.md).[metadata](Member.md#metadata)

___

### name

• `Optional` **name**: `string`

#### Inherited from

[Member](Member.md).[name](Member.md#name)

___

### onLeft

• **onLeft**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

[Member](Member.md).[onLeft](Member.md#onleft)

___

### onMetadataUpdated

• **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

#### Inherited from

[Member](Member.md).[onMetadataUpdated](Member.md#onmetadataupdated)

___

### publications

• **publications**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

[Member](Member.md).[publications](Member.md#publications)

___

### side

• **side**: [`MemberSide`](../modules.md#memberside)

#### Inherited from

[Member](Member.md).[side](Member.md#side)

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

[Member](Member.md).[status](Member.md#status)

___

### subscriptions

• **subscriptions**: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Inherited from

[Member](Member.md).[subscriptions](Member.md#subscriptions)

___

### subtype

• `Readonly` **subtype**: ``"person"``

#### Overrides

[Member](Member.md).[subtype](Member.md#subtype)

___

### type

• `Readonly` **type**: ``"person"``

#### Overrides

[Member](Member.md).[type](Member.md#type)

## Methods

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

[Member](Member.md).[updateMetadata](Member.md#updatemetadata)
