[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / SfuClientPlugin

# Class: SfuClientPlugin

## Hierarchy

- `SkyWayPlugin`

  ↳ **`SfuClientPlugin`**

## Table of contents

### Constructors

- [constructor](SfuClientPlugin.md#constructor)

### Properties

- [options](SfuClientPlugin.md#options)
- [subtype](SfuClientPlugin.md#subtype)

### Methods

- [createBot](SfuClientPlugin.md#createbot)
- [deleteBot](SfuClientPlugin.md#deletebot)

## Constructors

### constructor

• **new SfuClientPlugin**(`_options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_options` | `Partial`<[`SfuClientPluginOptions`](../modules.md#sfuclientpluginoptions)\> |

#### Overrides

SkyWayPlugin.constructor

## Properties

### options

• `Readonly` **options**: [`SfuClientPluginOptions`](../modules.md#sfuclientpluginoptions)

___

### subtype

• `Readonly` **subtype**: ``"sfu"``

#### Overrides

SkyWayPlugin.subtype

## Methods

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
