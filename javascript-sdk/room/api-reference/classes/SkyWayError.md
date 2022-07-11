[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / SkyWayError

# Class: SkyWayError<PayloadType\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `PayloadType` | extends `Record`<`string`, `any`\> = `Record`<`string`, `any`\> |

## Hierarchy

- `Error`

  ↳ **`SkyWayError`**

## Table of contents

### Properties

- [message](SkyWayError.md#message)
- [name](SkyWayError.md#name)
- [path](SkyWayError.md#path)
- [payload](SkyWayError.md#payload)
- [stack](SkyWayError.md#stack)
- [type](SkyWayError.md#type)
- [prepareStackTrace](SkyWayError.md#preparestacktrace)
- [stackTraceLimit](SkyWayError.md#stacktracelimit)

### Methods

- [toJSON](SkyWayError.md#tojson)
- [captureStackTrace](SkyWayError.md#capturestacktrace)

## Properties

### message

• **message**: `string`

#### Overrides

Error.message

___

### name

• **name**: `string`

#### Inherited from

Error.name

___

### path

• `Optional` **path**: `string`

___

### payload

• `Optional` **payload**: `PayloadType`

___

### stack

• `Optional` **stack**: `string`

#### Inherited from

Error.stack

___

### type

• **type**: `ErrorType`

___

### prepareStackTrace

▪ `Static` `Optional` **prepareStackTrace**: (`err`: `Error`, `stackTraces`: `CallSite`[]) => `any`

#### Type declaration

▸ (`err`, `stackTraces`): `any`

Optional override for formatting stack traces

**`see`** https://v8.dev/docs/stack-trace-api#customizing-stack-traces

##### Parameters

| Name | Type |
| :------ | :------ |
| `err` | `Error` |
| `stackTraces` | `CallSite`[] |

##### Returns

`any`

#### Inherited from

Error.prepareStackTrace

___

### stackTraceLimit

▪ `Static` **stackTraceLimit**: `number`

#### Inherited from

Error.stackTraceLimit

## Methods

### toJSON

▸ **toJSON**(): `Object`

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `message` | `string` |
| `payload` | `undefined` \| `PayloadType` |
| `type` | `ErrorType` |

___

### captureStackTrace

▸ `Static` **captureStackTrace**(`targetObject`, `constructorOpt?`): `void`

Create .stack property on a target object

#### Parameters

| Name | Type |
| :------ | :------ |
| `targetObject` | `object` |
| `constructorOpt?` | `Function` |

#### Returns

`void`

#### Inherited from

Error.captureStackTrace
