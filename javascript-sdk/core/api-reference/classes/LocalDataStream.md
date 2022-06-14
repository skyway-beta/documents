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

### Accessors

- [muted](LocalDataStream.md#muted)

### Methods

- [mute](LocalDataStream.md#mute)
- [unmute](LocalDataStream.md#unmute)
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

## Accessors

### muted

• `get` **muted**(): `boolean`

#### Returns

`boolean`

#### Inherited from

LocalStreamBase.muted

## Methods

### mute

▸ **mute**(): `void`

#### Returns

`void`

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[mute](LocalStreamBase.md#mute)

___

### unmute

▸ **unmute**(): `void`

#### Returns

`void`

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[unmute](LocalStreamBase.md#unmute)

___

### write

▸ **write**(`object`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `object` | `Object` |

#### Returns

`void`
