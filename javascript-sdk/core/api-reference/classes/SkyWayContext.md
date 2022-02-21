[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayContext

# Class: SkyWayContext

## Table of contents

### Properties

- [\_api](SkyWayContext.md#_api)
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

### \_api

• `Readonly` **\_api**: `RtcApiClient`

___

### appId

• `Readonly` **appId**: `string`

___

### authToken

• **authToken**: [`SkyWayAuthToken`](SkyWayAuthToken.md)

___

### onTokenExpired

• `Readonly` **onTokenExpired**: [`Event`](Event.md)<`void`\>

___

### onTokenUpdateReminder

• `Readonly` **onTokenUpdateReminder**: [`Event`](Event.md)<`void`\>

___

### plugins

• **plugins**: [`SkyWayPlugin`](SkyWayPlugin.md)[] = `[]`

## Accessors

### authTokenString

• `get` **authTokenString**(): `string`

#### Returns

`string`

___

### config

• `get` **config**(): [`SkyWayConfig`](SkyWayConfig.md)

#### Returns

[`SkyWayConfig`](SkyWayConfig.md)

## Methods

### registerPlugin

▸ **registerPlugin**(`plugin`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `plugin` | [`SkyWayPlugin`](SkyWayPlugin.md) |

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
| `configOptions` | `Partial`<[`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)\> |

#### Returns

`Promise`<[`SkyWayContext`](SkyWayContext.md)\>
