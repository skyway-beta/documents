[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / LocalDataStream

# Class: LocalDataStream

## Hierarchy

- [`LocalStreamBase`](LocalStreamBase.md)

  ↳ **`LocalDataStream`**

## Table of contents

### Constructors

- [constructor](LocalDataStream.md#constructor)

### Properties

- [\_options](LocalDataStream.md#_options)
- [contentType](LocalDataStream.md#contenttype)
- [id](LocalDataStream.md#id)
- [label](LocalDataStream.md#label)
- [side](LocalDataStream.md#side)

### Methods

- [write](LocalDataStream.md#write)

## Constructors

### constructor

• **new LocalDataStream**(`_options?`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `_options` | [`DataStreamOptions`](../interfaces/DataStreamOptions.md) |

#### Overrides

LocalStreamBase.constructor

## Properties

### \_options

• **\_options**: [`DataStreamOptions`](../interfaces/DataStreamOptions.md) = `{}`

___

### contentType

• `Readonly` **contentType**: ``"data"``

#### Overrides

[LocalStreamBase](LocalStreamBase.md).[contentType](LocalStreamBase.md#contenttype)

___

### id

• `Readonly` **id**: `string`

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[id](LocalStreamBase.md#id)

___

### label

• `Readonly` **label**: `string`

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[label](LocalStreamBase.md#label)

___

### side

• `Readonly` **side**: ``"local"``

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[side](LocalStreamBase.md#side)

## Methods

### write

▸ **write**(`data`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | [`DataStreamMessageType`](../modules.md#datastreammessagetype) |

#### Returns

`void`
