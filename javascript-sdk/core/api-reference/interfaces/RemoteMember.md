[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemoteMember

# Interface: RemoteMember

## Hierarchy

- [`Member`](Member.md)

  ↳ **`RemoteMember`**

## Table of contents

### Properties

- [channel](RemoteMember.md#channel)
- [id](RemoteMember.md#id)
- [metadata](RemoteMember.md#metadata)
- [name](RemoteMember.md#name)
- [onLeft](RemoteMember.md#onleft)
- [onMetadataUpdated](RemoteMember.md#onmetadataupdated)
- [publications](RemoteMember.md#publications)
- [side](RemoteMember.md#side)
- [status](RemoteMember.md#status)
- [subscriptions](RemoteMember.md#subscriptions)
- [subtype](RemoteMember.md#subtype)
- [type](RemoteMember.md#type)

### Methods

- [updateMetadata](RemoteMember.md#updatemetadata)

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

• `Readonly` **side**: ``"remote"``

#### Overrides

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

• **subtype**: `string`

#### Inherited from

[Member](Member.md).[subtype](Member.md#subtype)

___

### type

• **type**: [`MemberType`](../modules.md#membertype)

#### Inherited from

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
