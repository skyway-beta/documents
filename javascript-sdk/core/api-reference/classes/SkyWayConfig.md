[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayConfig

# Class: SkyWayConfig

## Implements

- [`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)

## Table of contents

### Properties

- [iceParamServer](SkyWayConfig.md#iceparamserver)
- [logLevel](SkyWayConfig.md#loglevel)
- [messageService](SkyWayConfig.md#messageservice)
- [rtcApi](SkyWayConfig.md#rtcapi)
- [rtcConfig](SkyWayConfig.md#rtcconfig)

### Accessors

- [get](SkyWayConfig.md#get)

### Methods

- [initialize](SkyWayConfig.md#initialize)

## Properties

### iceParamServer

• **iceParamServer**: `Required`<{ `url?`: `string`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[iceParamServer](../interfaces/SkyWayConfigOptions.md#iceparamserver)

___

### logLevel

• **logLevel**: ``"error"`` \| ``"warn"`` \| ``"debug"`` \| ``"disable"`` = `'error'`

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[logLevel](../interfaces/SkyWayConfigOptions.md#loglevel)

___

### messageService

• **messageService**: `Required`<{ `domain?`: `string`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[messageService](../interfaces/SkyWayConfigOptions.md#messageservice)

___

### rtcApi

• **rtcApi**: `Required`<{ `apiVersion?`: `string` ; `host?`: `string` ; `secure?`: `boolean` ; `timeout?`: `number`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[rtcApi](../interfaces/SkyWayConfigOptions.md#rtcapi)

___

### rtcConfig

• **rtcConfig**: `Required`<{ `encodedInsertableStreams?`: `boolean` ; `timeout?`: `number` ; `turnPolicy?`: [`TurnPolicy`](../modules.md#turnpolicy)  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[rtcConfig](../interfaces/SkyWayConfigOptions.md#rtcconfig)

## Accessors

### get

• `Static` `get` **get**(): [`SkyWayConfig`](SkyWayConfig.md)

#### Returns

[`SkyWayConfig`](SkyWayConfig.md)

## Methods

### initialize

▸ `Static` **initialize**(`options?`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Partial`<[`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)\> |

#### Returns

`void`
