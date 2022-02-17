[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / SfuClientPlugin

# Class: SfuClientPlugin

## Hierarchy

- `SkyWayPlugin`

  ↳ **`SfuClientPlugin`**

## Table of contents

### Constructors

- [constructor](SfuClientPlugin.md#constructor)

### Properties

- [\_context](SfuClientPlugin.md#_context)
- [\_onContextAttached](SfuClientPlugin.md#_oncontextattached)
- [\_whenCreateLocalPerson](SfuClientPlugin.md#_whencreatelocalperson)
- [\_whenDisposeLocalPerson](SfuClientPlugin.md#_whendisposelocalperson)
- [subtype](SfuClientPlugin.md#subtype)

### Methods

- [\_attachContext](SfuClientPlugin.md#_attachcontext)
- [createBot](SfuClientPlugin.md#createbot)
- [deleteBot](SfuClientPlugin.md#deletebot)

## Constructors

### constructor

• **new SfuClientPlugin**(`_options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_options` | [`SfuClientPluginOptions`](../interfaces/SfuClientPluginOptions.md) |

#### Overrides

SkyWayPlugin.constructor

## Properties

### \_context

• **\_context**: `SkyWayContext`

#### Inherited from

SkyWayPlugin.\_context

___

### \_onContextAttached

• **\_onContextAttached**: `Event`<`void`\>

#### Inherited from

SkyWayPlugin.\_onContextAttached

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

#### Inherited from

SkyWayPlugin.\_whenCreateLocalPerson

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

#### Inherited from

SkyWayPlugin.\_whenDisposeLocalPerson

___

### subtype

• `Readonly` **subtype**: ``"sfu"``

#### Overrides

SkyWayPlugin.subtype

## Methods

### \_attachContext

▸ **_attachContext**(`context`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | `SkyWayContext` |

#### Returns

`void`

#### Inherited from

SkyWayPlugin.\_attachContext

___

### createBot

▸ **createBot**(`channel`): `Promise`<[`SfuBotMember`](SfuBotMember.md)\>

**`description`** {japanese} SFU BotをChannelに呼び出す

#### Parameters

| Name | Type |
| :------ | :------ |
| `channel` | `Channel` |

#### Returns

`Promise`<[`SfuBotMember`](SfuBotMember.md)\>

___

### deleteBot

▸ **deleteBot**(`channel`, `botId`): `Promise`<`void`\>

**`description`** {japanese} SFU BotをChannelから削除する

#### Parameters

| Name | Type |
| :------ | :------ |
| `channel` | `Channel` |
| `botId` | `string` |

#### Returns

`Promise`<`void`\>
