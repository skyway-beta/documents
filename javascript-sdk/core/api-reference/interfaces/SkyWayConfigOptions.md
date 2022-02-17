[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayConfigOptions

# Interface: SkyWayConfigOptions

## Implemented by

- [`SkyWayConfig`](../classes/SkyWayConfig.md)

## Table of contents

### Properties

- [iceParamServer](SkyWayConfigOptions.md#iceparamserver)
- [logLevel](SkyWayConfigOptions.md#loglevel)
- [messageService](SkyWayConfigOptions.md#messageservice)
- [rtcApi](SkyWayConfigOptions.md#rtcapi)
- [rtcConfig](SkyWayConfigOptions.md#rtcconfig)

## Properties

### iceParamServer

• **iceParamServer**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `url?` | `string` |

___

### logLevel

• `Optional` **logLevel**: ``"error"`` \| ``"warn"`` \| ``"debug"`` \| ``"disable"``

___

### messageService

• **messageService**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `domain?` | `string` |

___

### rtcApi

• **rtcApi**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `apiVersion?` | `string` |
| `host?` | `string` |
| `secure?` | `boolean` |
| `timeout?` | `number` |

___

### rtcConfig

• **rtcConfig**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `encodedInsertableStreams?` | `boolean` |
| `timeout?` | `number` |
| `turnPolicy?` | [`TurnPolicy`](../modules.md#turnpolicy) |