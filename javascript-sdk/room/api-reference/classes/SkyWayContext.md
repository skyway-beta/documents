[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / SkyWayContext

# Class: SkyWayContext

## Table of contents

### Properties

- [appId](SkyWayContext.md#appid)
- [authToken](SkyWayContext.md#authtoken)
- [onTokenExpired](SkyWayContext.md#ontokenexpired)
- [onTokenUpdateReminder](SkyWayContext.md#ontokenupdatereminder)
- [plugins](SkyWayContext.md#plugins)

### Accessors

- [authTokenString](SkyWayContext.md#authtokenstring)
- [config](SkyWayContext.md#config)

### Methods

- [registerPlugin](SkyWayContext.md#registerplugin)
- [updateAuthToken](SkyWayContext.md#updateauthtoken)
- [Create](SkyWayContext.md#create)

## Properties

### appId

• `Readonly` **appId**: `string`

___

### authToken

• **authToken**: [`SkyWayAuthToken`](SkyWayAuthToken.md)

___

### onTokenExpired

• `Readonly` **onTokenExpired**: `Event`<`void`\>

___

### onTokenUpdateReminder

• `Readonly` **onTokenUpdateReminder**: `Event`<`void`\>

___

### plugins

• **plugins**: `SkyWayPlugin`[]

## Accessors

### authTokenString

• `get` **authTokenString**(): `string`

#### Returns

`string`

___

### config

• `get` **config**(): `SkyWayConfig`

#### Returns

`SkyWayConfig`

## Methods

### registerPlugin

▸ **registerPlugin**(`plugin`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `plugin` | `SkyWayPlugin` |

#### Returns

`void`

___

### updateAuthToken

▸ **updateAuthToken**(`token`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | `string` |

#### Returns

`void`

___

### Create

▸ `Static` **Create**(`authTokenString`, `configOptions?`): `Promise`<[`SkyWayContext`](SkyWayContext.md)\>

**`description`** {japanese} Contextの作成

#### Parameters

| Name | Type |
| :------ | :------ |
| `authTokenString` | `string` |
| `configOptions?` | `Partial`<[`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)\> |

#### Returns

`Promise`<[`SkyWayContext`](SkyWayContext.md)\>
