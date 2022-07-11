[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / SfuBotMember

# Class: SfuBotMember

## Hierarchy

- `MemberImpl`

  ↳ **`SfuBotMember`**

## Implements

- `RemoteMemberImplInterface`

## Table of contents

### Properties

- [channel](SfuBotMember.md#channel)
- [id](SfuBotMember.md#id)
- [name](SfuBotMember.md#name)
- [onForwardingStarted](SfuBotMember.md#onforwardingstarted)
- [onForwardingStateChanged](SfuBotMember.md#onforwardingstatechanged)
- [onForwardingStopped](SfuBotMember.md#onforwardingstopped)
- [onLeft](SfuBotMember.md#onleft)
- [onMetadataUpdated](SfuBotMember.md#onmetadataupdated)
- [side](SfuBotMember.md#side)
- [subtype](SfuBotMember.md#subtype)
- [type](SfuBotMember.md#type)
- [subtype](SfuBotMember.md#subtype-1)

### Accessors

- [forwardings](SfuBotMember.md#forwardings)
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

### channel

• `Readonly` **channel**: `SkyWayChannelImpl`

#### Implementation of

RemoteMemberImplInterface.channel

#### Inherited from

MemberImpl.channel

___

### id

• `Readonly` **id**: `string`

#### Implementation of

RemoteMemberImplInterface.id

#### Inherited from

MemberImpl.id

___

### name

• `Optional` `Readonly` **name**: `string`

#### Implementation of

RemoteMemberImplInterface.name

#### Inherited from

MemberImpl.name

___

### onForwardingStarted

• `Readonly` **onForwardingStarted**: `Event`<{ `forwarding`: [`Forwarding`](Forwarding.md)  }\>

___

### onForwardingStateChanged

• `Readonly` **onForwardingStateChanged**: `Event`<`void`\>

___

### onForwardingStopped

• `Readonly` **onForwardingStopped**: `Event`<{ `forwarding`: [`Forwarding`](Forwarding.md)  }\>

___

### onLeft

• `Readonly` **onLeft**: `Event`<`void`\>

#### Implementation of

RemoteMemberImplInterface.onLeft

#### Inherited from

MemberImpl.onLeft

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: `Event`<`string`\>

#### Implementation of

RemoteMemberImplInterface.onMetadataUpdated

#### Inherited from

MemberImpl.onMetadataUpdated

___

### side

• `Readonly` **side**: ``"remote"``

#### Implementation of

RemoteMemberImplInterface.side

#### Overrides

MemberImpl.side

___

### subtype

• `Readonly` **subtype**: ``"sfu"``

#### Implementation of

RemoteMemberImplInterface.subtype

#### Overrides

MemberImpl.subtype

___

### type

• `Readonly` **type**: `MemberType` = `'bot'`

#### Implementation of

RemoteMemberImplInterface.type

#### Overrides

MemberImpl.type

___

### subtype

▪ `Static` `Readonly` **subtype**: ``"sfu"``

## Accessors

### forwardings

• `get` **forwardings**(): [`Forwarding`](Forwarding.md)[]

#### Returns

[`Forwarding`](Forwarding.md)[]

___

### metadata

• `get` **metadata**(): `undefined` \| `string`

#### Returns

`undefined` \| `string`

#### Implementation of

RemoteMemberImplInterface.metadata

#### Inherited from

MemberImpl.metadata

___

### publications

• `get` **publications**(): `Publication`<`LocalStream`\>[]

#### Returns

`Publication`<`LocalStream`\>[]

#### Implementation of

RemoteMemberImplInterface.publications

#### Inherited from

MemberImpl.publications

___

### status

• `get` **status**(): `MemberStatus`

#### Returns

`MemberStatus`

#### Implementation of

RemoteMemberImplInterface.status

#### Inherited from

MemberImpl.status

___

### subscriptions

• `get` **subscriptions**(): `Subscription`<`RemoteStream`\>[]

#### Returns

`Subscription`<`RemoteStream`\>[]

#### Implementation of

RemoteMemberImplInterface.subscriptions

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

▸ **stopForwarding**(`target`): `Promise`<`void`\>

**`description`** {japanese} Forwardingを停止する

#### Parameters

| Name | Type |
| :------ | :------ |
| `target` | `string` \| [`Forwarding`](Forwarding.md) |

#### Returns

`Promise`<`void`\>

___

### toJSON

▸ **toJSON**(): `Member`

#### Returns

`Member`

#### Implementation of

RemoteMemberImplInterface.toJSON

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

RemoteMemberImplInterface.updateMetadata

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
