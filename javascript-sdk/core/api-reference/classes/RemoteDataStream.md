[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemoteDataStream

# Class: RemoteDataStream

## Hierarchy

- `RemoteStreamBase`

  ↳ **`RemoteDataStream`**

## Table of contents

### Constructors

- [constructor](RemoteDataStream.md#constructor)

### Properties

- [\_datachannel](RemoteDataStream.md#_datachannel)
- [contentType](RemoteDataStream.md#contenttype)
- [id](RemoteDataStream.md#id)
- [label](RemoteDataStream.md#label)
- [onData](RemoteDataStream.md#ondata)
- [side](RemoteDataStream.md#side)

## Constructors

### constructor

• **new RemoteDataStream**(`id`, `label`, `_datachannel`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `label` | `string` |
| `_datachannel` | `RTCDataChannel` |

#### Overrides

RemoteStreamBase.constructor

## Properties

### \_datachannel

• **\_datachannel**: `RTCDataChannel`

___

### contentType

• `Readonly` **contentType**: ``"data"``

#### Overrides

RemoteStreamBase.contentType

___

### id

• `Readonly` **id**: `string`

#### Inherited from

RemoteStreamBase.id

___

### label

• `Readonly` **label**: `string`

#### Inherited from

RemoteStreamBase.label

___

### onData

• `Readonly` **onData**: [`Event`](Event.md)<`Record`<`string`, `any`\>\>

___

### side

• `Readonly` **side**: ``"remote"``

#### Inherited from

RemoteStreamBase.side
