[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / SfuBotMember

# Class: SfuBotMember

## Hierarchy

- `MemberImpl`

  ↳ **`SfuBotMember`**

## Implements

- `RemoteMember`

## Table of contents

### Properties

- [\_events](SfuBotMember.md#_events)
- [channel](SfuBotMember.md#channel)
- [id](SfuBotMember.md#id)
- [name](SfuBotMember.md#name)
- [onForwardingStarted](SfuBotMember.md#onforwardingstarted)
- [onForwardingStateChanged](SfuBotMember.md#onforwardingstatechanged)
- [onForwardingStopped](SfuBotMember.md#onforwardingstopped)
- [onJoined](SfuBotMember.md#onjoined)
- [onLeft](SfuBotMember.md#onleft)
- [onMembershipChanged](SfuBotMember.md#onmembershipchanged)
- [onMetadataUpdated](SfuBotMember.md#onmetadataupdated)
- [side](SfuBotMember.md#side)
- [subtype](SfuBotMember.md#subtype)
- [type](SfuBotMember.md#type)
- [subtype](SfuBotMember.md#subtype)

### Accessors

- [metadata](SfuBotMember.md#metadata)
- [publications](SfuBotMember.md#publications)
- [status](SfuBotMember.md#status)
- [subscriptions](SfuBotMember.md#subscriptions)

### Methods

- [startForwarding](SfuBotMember.md#startforwarding)
- [stopForwarding](SfuBotMember.md#stopforwarding)
- [toJSON](SfuBotMember.md#tojson)
- [updateMetadata](SfuBotMember.md#updatemetadata)
- [IsSfuBotMember](SfuBotMember.md#issfubotmember)

## Properties

### \_events

• `Readonly` **\_events**: `Events`

#### Inherited from

MemberImpl.\_events

___

### channel

• `Readonly` **channel**: `SkyWayChannelImpl`

#### Implementation of

RemoteMember.channel

#### Inherited from

MemberImpl.channel

___

### id

• `Readonly` **id**: `string`

#### Implementation of

RemoteMember.id

#### Inherited from

MemberImpl.id

___

### name

• `Optional` `Readonly` **name**: `string`

#### Implementation of

RemoteMember.name

#### Inherited from

MemberImpl.name

___

### onForwardingStarted

• `Readonly` **onForwardingStarted**: `Event`<[`Forwarding`](Forwarding.md)\>

___

### onForwardingStateChanged

• `Readonly` **onForwardingStateChanged**: `Event`<`void`\>

___

### onForwardingStopped

• `Readonly` **onForwardingStopped**: `Event`<[`Forwarding`](Forwarding.md)\>

___

### onJoined

• `Readonly` **onJoined**: `Event`<`void`\>

#### Implementation of

RemoteMember.onJoined

#### Inherited from

MemberImpl.onJoined

___

### onLeft

• `Readonly` **onLeft**: `Event`<`void`\>

#### Implementation of

RemoteMember.onLeft

#### Inherited from

MemberImpl.onLeft

___

### onMembershipChanged

• `Readonly` **onMembershipChanged**: `Event`<`void`\>

#### Implementation of

RemoteMember.onMembershipChanged

#### Inherited from

MemberImpl.onMembershipChanged

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<`string`\>

#### Implementation of

RemoteMember.onMetadataUpdated

#### Inherited from

MemberImpl.onMetadataUpdated

___

### side

• `Readonly` **side**: ``"remote"``

#### Implementation of

RemoteMember.side

#### Overrides

MemberImpl.side

___

### subtype

• `Readonly` **subtype**: ``"sfu"``

#### Implementation of

RemoteMember.subtype

#### Overrides

MemberImpl.subtype

___

### type

• `Readonly` **type**: `MemberType` = `'bot'`

#### Implementation of

RemoteMember.type

#### Overrides

MemberImpl.type

___

### subtype

▪ `Static` `Readonly` **subtype**: ``"sfu"``

## Accessors

### metadata

• `get` **metadata**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Implementation of

RemoteMember.metadata

#### Inherited from

MemberImpl.metadata

___

### publications

• `get` **publications**(): `Publication`<`LocalStream`\>[]

#### Returns

`Publication`<`LocalStream`\>[]

#### Implementation of

RemoteMember.publications

#### Inherited from

MemberImpl.publications

___

### status

• `get` **status**(): `MemberStatus`

#### Returns

`MemberStatus`

#### Implementation of

RemoteMember.status

#### Inherited from

MemberImpl.status

___

### subscriptions

• `get` **subscriptions**(): `Subscription`<`RemoteStream`\>[]

#### Returns

`Subscription`<`RemoteStream`\>[]

#### Implementation of

RemoteMember.subscriptions

#### Inherited from

MemberImpl.subscriptions

## Methods

### startForwarding

▸ **startForwarding**(`publication`, `configure?`): `Promise`<[`Forwarding`](Forwarding.md)\>

**`description`** {japanese} StreamのPublicationをForwardingする

#### Parameters

| Name | Type |
| :------ | :------ |
| `publication` | `Publication`<`LocalAudioStream` \| `LocalVideoStream`\> |
| `configure` | [`ForwardingConfigure`](../interfaces/ForwardingConfigure.md) |

#### Returns

`Promise`<[`Forwarding`](Forwarding.md)\>

___

### stopForwarding

▸ **stopForwarding**(`forwardingId`): `Promise`<`void`\>

**`description`** {japanese} Forwardingを停止する

#### Parameters

| Name | Type |
| :------ | :------ |
| `forwardingId` | `string` |

#### Returns

`Promise`<`void`\>

___

### toJSON

▸ **toJSON**(): `Member`

#### Returns

`Member`

#### Inherited from

MemberImpl.toJSON

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

RemoteMember.updateMetadata

#### Inherited from

MemberImpl.updateMetadata

___

### IsSfuBotMember

▸ `Static` **IsSfuBotMember**(`member`): member is SfuBotMember

**`description`** {japanese} MemberがSfuBotかどうか識別する

#### Parameters

| Name | Type |
| :------ | :------ |
| `member` | `Member` |

#### Returns

member is SfuBotMember
