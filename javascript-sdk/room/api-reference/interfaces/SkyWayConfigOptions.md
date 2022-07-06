[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / SkyWayConfigOptions

# Interface: SkyWayConfigOptions

## Table of contents

### Properties

- [debug](SkyWayConfigOptions.md#debug)
- [iceParamServer](SkyWayConfigOptions.md#iceparamserver)
- [log](SkyWayConfigOptions.md#log)
- [messageService](SkyWayConfigOptions.md#messageservice)
- [rtcApi](SkyWayConfigOptions.md#rtcapi)
- [rtcConfig](SkyWayConfigOptions.md#rtcconfig)
- [token](SkyWayConfigOptions.md#token)

## Properties

### debug

• **debug**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `disableDPlane?` | `boolean` |

___

### iceParamServer

• **iceParamServer**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `domain?` | `string` |
| `secure?` | `boolean` |
| `version?` | `number` |

___

### log

• **log**: `Partial`<{ `format`: [`LogFormat`](../modules.md#logformat) ; `level`: ``"error"`` \| ``"disable"`` \| ``"warn"`` \| ``"debug"``  }\>

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
