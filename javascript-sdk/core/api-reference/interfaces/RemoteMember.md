[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemoteMember

# Interface: RemoteMember

## Hierarchy

- `MemberImpl`

  ↳ **`RemoteMember`**

## Table of contents

### Properties

- [\_events](RemoteMember.md#_events)
- [channel](RemoteMember.md#channel)
- [id](RemoteMember.md#id)
- [name](RemoteMember.md#name)
- [onJoined](RemoteMember.md#onjoined)
- [onLeft](RemoteMember.md#onleft)
- [onMembershipChanged](RemoteMember.md#onmembershipchanged)
- [onMetadataUpdated](RemoteMember.md#onmetadataupdated)
- [side](RemoteMember.md#side)
- [subtype](RemoteMember.md#subtype)
- [type](RemoteMember.md#type)

### Accessors

- [\_dto](RemoteMember.md#_dto)
- [metadata](RemoteMember.md#metadata)
- [publications](RemoteMember.md#publications)
- [status](RemoteMember.md#status)
- [subscriptions](RemoteMember.md#subscriptions)

### Methods

- [\_getConnection](RemoteMember.md#_getconnection)
- [\_getOrCreateConnection](RemoteMember.md#_getorcreateconnection)
- [updateMetadata](RemoteMember.md#updatemetadata)

## Properties

### \_events

• `Readonly` **\_events**: `Events`

#### Inherited from

MemberImpl.\_events

___

### channel

• `Readonly` **channel**: [`SkyWayChannel`](../classes/SkyWayChannel.md)

#### Inherited from

MemberImpl.channel

___

### id

• `Readonly` **id**: `string`

#### Inherited from

MemberImpl.id

___

### name

• `Optional` `Readonly` **name**: `string`

#### Inherited from

MemberImpl.name

___

### onJoined

• `Readonly` **onJoined**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

MemberImpl.onJoined

___

### onLeft

• `Readonly` **onLeft**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

MemberImpl.onLeft

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: [`Event`](../classes/Event.md)<`void`\>

#### Inherited from

MemberImpl.onMembershipChanged

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](../classes/Event.md)<`string`\>

#### Inherited from

MemberImpl.onMetadataUpdated

___

### side

• `Readonly` **side**: ``"remote"``

#### Overrides

MemberImpl.side

___

### subtype

• `Readonly` **subtype**: `string`

#### Inherited from

MemberImpl.subtype

___

### type

• `Readonly` **type**: [`MemberType`](../modules.md#membertype)

#### Inherited from

MemberImpl.type

## Accessors

### \_dto

• `get` **_dto**(): `Member`

#### Returns

`Member`

#### Inherited from

MemberImpl.\_dto

___

### metadata

• `get` **metadata**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Inherited from

MemberImpl.metadata

___

### publications

• `get` **publications**(): [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Returns

[`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>[]

#### Inherited from

MemberImpl.publications

___

### status

• `get` **status**(): [`MemberStatus`](../modules.md#memberstatus)

#### Returns

[`MemberStatus`](../modules.md#memberstatus)

#### Inherited from

MemberImpl.status

___

### subscriptions

• `get` **subscriptions**(): [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Returns

[`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

#### Inherited from

MemberImpl.subscriptions

## Methods

### \_getConnection

▸ **_getConnection**(`localPersonId`): `undefined` \| [`SkyWayConnection`](SkyWayConnection.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `localPersonId` | `string` |

#### Returns

`undefined` \| [`SkyWayConnection`](SkyWayConnection.md)

___

### \_getOrCreateConnection

▸ **_getOrCreateConnection**(`localPersonId`): [`SkyWayConnection`](SkyWayConnection.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `localPersonId` | `string` |

#### Returns

[`SkyWayConnection`](SkyWayConnection.md)

___

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>

#### Inherited from

MemberImpl.updateMetadata
