[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / SkyWayConfig

# Class: SkyWayConfig

## Implements

- [`SkyWayConfigOptions`](../interfaces/SkyWayConfigOptions.md)

## Table of contents

### Properties

- [debug](SkyWayConfig.md#debug)
- [iceParamServer](SkyWayConfig.md#iceparamserver)
- [log](SkyWayConfig.md#log)
- [messageService](SkyWayConfig.md#messageservice)
- [rtcApi](SkyWayConfig.md#rtcapi)
- [rtcConfig](SkyWayConfig.md#rtcconfig)
- [token](SkyWayConfig.md#token)

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

### log

• **log**: `Required`<`Partial`<{ `format`: [`LogFormat`](../modules.md#logformat) ; `level`: ``"disable"`` \| ``"error"`` \| ``"warn"`` \| ``"debug"``  }\>\>

#### Implementation of

[SkyWayConfigOptions](../interfaces/SkyWayConfigOptions.md).[log](../interfaces/SkyWayConfigOptions.md#log)

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
