[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Member

# Interface: Member

## Hierarchy

- **`Member`**

  ↳ [`RemoteMember`](RemoteMember.md)

## Table of contents

### Properties

- [channel](Member.md#channel)
- [id](Member.md#id)
- [metadata](Member.md#metadata)
- [name](Member.md#name)
- [onJoined](Member.md#onjoined)
- [onLeft](Member.md#onleft)
- [onMembershipChanged](Member.md#onmembershipchanged)
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

### onJoined

• **onJoined**: [`Event`](../classes/Event.md)<`void`\>

___

### onLeft

• **onLeft**: [`Event`](../classes/Event.md)<`void`\>

___

### onMembershipChanged

• **onMembershipChanged**: [`Event`](../classes/Event.md)<`void`\>

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
