[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayConfig

# Class: SkyWayConfig

## Implements

- [`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)

## Table of contents

### Properties

- [debug](SkyWayConfig.md#debug)
- [iceParamServer](SkyWayConfig.md#iceparamserver)
- [logLevel](SkyWayConfig.md#loglevel)
- [messageService](SkyWayConfig.md#messageservice)
- [rtcApi](SkyWayConfig.md#rtcapi)
- [rtcConfig](SkyWayConfig.md#rtcconfig)
- [token](SkyWayConfig.md#token)

### Accessors

- [get](SkyWayConfig.md#get)

### Methods

- [initialize](SkyWayConfig.md#initialize)

## Properties

### debug

• **debug**: `Required`<{ `disableDPlane?`: `boolean`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[debug](../interfaces/SkyWayConfigOptions.md#debug)

___

### iceParamServer

• **iceParamServer**: `Required`<{ `domain?`: `string` ; `secure?`: `boolean` ; `version?`: `number`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[iceParamServer](../interfaces/SkyWayConfigOptions.md#iceparamserver)

___

### logLevel

• **logLevel**: ``"disable"`` \| ``"error"`` \| ``"warn"`` \| ``"debug"`` = `'error'`

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[logLevel](../interfaces/SkyWayConfigOptions.md#loglevel)

___

### messageService

• **messageService**: `Required`<{ `domain?`: `string` ; `secure?`: `boolean`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[messageService](../interfaces/SkyWayConfigOptions.md#messageservice)

___

### rtcApi

• **rtcApi**: `Required`<[`RtcRpcApiConfig`](../interfaces/RtcRpcApiConfig.md)\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[rtcApi](../interfaces/SkyWayConfigOptions.md#rtcapi)

___

### rtcConfig

• **rtcConfig**: `Required`<{ `encodedInsertableStreams?`: `boolean` ; `timeout?`: `number` ; `turnPolicy?`: [`TurnPolicy`](../modules.md#turnpolicy)  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[rtcConfig](../interfaces/SkyWayConfigOptions.md#rtcconfig)

___

### token

• **token**: `Required`<{ `updateReminderSec?`: `number`  }\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[token](../interfaces/SkyWayConfigOptions.md#token)

## Accessors

### get

• `Static` `get` **get**(): [`SkyWayConfig`](SkyWayConfig.md)

#### Returns

[`SkyWayConfig`](SkyWayConfig.md)

## Methods

### initialize

▸ `Static` **initialize**(`options?`): [`SkyWayConfig`](SkyWayConfig.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `Partial`<[`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)\> |

#### Returns

[`SkyWayConfig`](SkyWayConfig.md)
