[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalDataStream

# Class: LocalDataStream

## Hierarchy

- `LocalStreamBase`

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
| `_options?` | `DataStreamOptions` |

#### Overrides

LocalStreamBase.constructor

## Properties

### \_options

• **\_options**: `DataStreamOptions`

___

### contentType

• `Readonly` **contentType**: ``"data"``

#### Overrides

LocalStreamBase.contentType

___

### id

• `Readonly` **id**: `string`

#### Inherited from

LocalStreamBase.id

___

### label

• `Readonly` **label**: `string`

#### Inherited from

LocalStreamBase.label

___

### side

• `Readonly` **side**: ``"local"``

#### Inherited from

LocalStreamBase.side

## Methods

### write

▸ **write**(`data`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `data` | `DataStreamMessageType` |

#### Returns

`void`
