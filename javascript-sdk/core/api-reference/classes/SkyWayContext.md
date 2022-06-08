[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayContext

# Class: SkyWayContext

## Table of contents

### Properties

- [appId](SkyWayContext.md#appid)
- [authToken](SkyWayContext.md#authtoken)
- [config](SkyWayContext.md#config)
- [disposed](SkyWayContext.md#disposed)
- [onFatalError](SkyWayContext.md#onfatalerror)
- [onTokenExpired](SkyWayContext.md#ontokenexpired)
- [onTokenUpdateReminder](SkyWayContext.md#ontokenupdatereminder)

### Accessors

- [authTokenString](SkyWayContext.md#authtokenstring)

### Methods

- [dispose](SkyWayContext.md#dispose)
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

### config

• **config**: [`SkyWayConfig`](SkyWayConfig.md)

___

### disposed

• **disposed**: `boolean` = `false`

___

### onFatalError

• `Readonly` **onFatalError**: [`Event`](Event.md)<[`SkyWayError`](SkyWayError.md)<`Record`<`string`, `any`\>\>\>

___

### onTokenExpired

• `Readonly` **onTokenExpired**: [`Event`](Event.md)<`void`\>

___

### onTokenUpdateReminder

• `Readonly` **onTokenUpdateReminder**: [`Event`](Event.md)<`void`\>

## Accessors

### authTokenString

• `get` **authTokenString**(): `string`

#### Returns

`string`

## Methods

### dispose

▸ **dispose**(): `void`

#### Returns

`void`

___

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
| `configOptions` | `Partial`<[`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)\> |

#### Returns

`Promise`<[`SkyWayContext`](SkyWayContext.md)\>
