[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Member

# Interface: Member

## Hierarchy

- **`Member`**

  ↳ [`Person`](Person.md)

  ↳ [`RemoteMember`](RemoteMember.md)

## Table of contents

### Properties

- [channel](Member.md#channel)
- [id](Member.md#id)
- [metadata](Member.md#metadata)
- [name](Member.md#name)
- [onLeft](Member.md#onleft)
- [onMetadataUpdated](Member.md#onmetadataupdated)
- [publications](Member.md#publications)
- [side](Member.md#side)
- [status](Member.md#status)
- [subscriptions](Member.md#subscriptions)
- [subtype](Member.md#subtype)
- [type](Member.md#type)

### Methods

- [updateMetadata](Member.md#updatemetadata)

## Properties

### channel

• **channel**: [`Channel`](Channel.md)

___

### id

• **id**: `string`

___

### metadata

• `Optional` **metadata**: `string`

___

### name

• `Optional` **name**: `string`

___

### onLeft

• **onLeft**: [`Event`](../classes/Event.md)<`void`\>

___

### onMetadataUpdated

• **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

___

### publications

• **publications**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

___

### side

• **side**: [`MemberSide`](../modules.md#memberside)

___

### status

• **status**: [`MemberStatus`](../modules.md#memberstatus)

___

### subscriptions

• **subscriptions**: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

___

### subtype

• **subtype**: `string`

___

### type

• **type**: [`MemberType`](../modules.md#membertype)

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
