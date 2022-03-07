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
- [token](SkyWayConfigOptions.md#token)

## Properties

### iceParamServer

• **iceParamServer**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `domain?` | `string` |
| `secure?` | `boolean` |
| `version?` | `number` |

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
| `secure?` | `boolean` |

___

### rtcApi

• **rtcApi**: [`RtcRpcApiConfig`](RtcRpcApiConfig.md)

___

### rtcConfig

• **rtcConfig**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `encodedInsertableStreams?` | `boolean` |
| `timeout?` | `number` |
| `turnPolicy?` | [`TurnPolicy`](../modules.md#turnpolicy) |

___

### token

• **token**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `updateReminderSec?` | `number` |
