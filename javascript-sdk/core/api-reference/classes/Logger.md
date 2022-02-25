[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Logger

# Class: Logger

## Table of contents

### Constructors

- [constructor](Logger.md#constructor)

### Properties

- [id](Logger.md#id)
- [level](Logger.md#level)
- [onLog](Logger.md#onlog)

### Methods

- [debug](Logger.md#debug)
- [error](Logger.md#error)
- [warn](Logger.md#warn)

## Constructors

### constructor

• **new Logger**(`_prefix`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_prefix` | `string` |

## Properties

### id

▪ `Static` `Readonly` **id**: `string`

___

### level

▪ `Static` **level**: ``"error"`` \| ``"warn"`` \| ``"debug"`` \| ``"disable"``

___

### onLog

▪ `Static` `Readonly` **onLog**: [`Event`](Event.md)<{ `id`: `string` ; `level`: `string` ; `message`: `any`[]  }\>

## Methods

### debug

▸ **debug**(...`msg`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...msg` | `any`[] |

#### Returns

`void`

___

### error

▸ **error**(...`msg`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...msg` | `any`[] |

#### Returns

`void`

___

### warn

▸ **warn**(...`msg`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `...msg` | `any`[] |

#### Returns

`void`
