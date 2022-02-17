[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayPlugin

# Class: SkyWayPlugin

## Table of contents

### Constructors

- [constructor](SkyWayPlugin.md#constructor)

### Properties

- [\_context](SkyWayPlugin.md#_context)
- [\_onContextAttached](SkyWayPlugin.md#_oncontextattached)
- [\_whenCreateLocalPerson](SkyWayPlugin.md#_whencreatelocalperson)
- [\_whenDisposeLocalPerson](SkyWayPlugin.md#_whendisposelocalperson)
- [subtype](SkyWayPlugin.md#subtype)

### Methods

- [\_attachContext](SkyWayPlugin.md#_attachcontext)
- [\_createRemoteMember](SkyWayPlugin.md#_createremotemember)

## Constructors

### constructor

• **new SkyWayPlugin**()

## Properties

### \_context

• **\_context**: [`SkyWayContext`](SkyWayContext.md)

___

### \_onContextAttached

• **\_onContextAttached**: [`Event`](Event.md)<`void`\>

___

### \_whenCreateLocalPerson

• `Optional` **\_whenCreateLocalPerson**: (`member`: `LocalPersonImpl`) => `Promise`<`void`\>

#### Type declaration

▸ (`member`): `Promise`<`void`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `member` | `LocalPersonImpl` |

##### Returns

`Promise`<`void`\>

___

### \_whenDisposeLocalPerson

• `Optional` **\_whenDisposeLocalPerson**: (`member`: `LocalPersonImpl`) => `Promise`<`void`\>

#### Type declaration

▸ (`member`): `Promise`<`void`\>

##### Parameters

| Name | Type |
| :------ | :------ |
| `member` | `LocalPersonImpl` |

##### Returns

`Promise`<`void`\>

___

### subtype

• **subtype**: `string`

## Methods

### \_attachContext

▸ **_attachContext**(`context`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |

#### Returns

`void`

___

### \_createRemoteMember

▸ `Abstract` **_createRemoteMember**(`channel`, `memberDto`): [`RemoteMember`](../interfaces/RemoteMember.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `channel` | [`SkyWayChannel`](SkyWayChannel.md) |
| `memberDto` | `Member` |

#### Returns

[`RemoteMember`](../interfaces/RemoteMember.md)
