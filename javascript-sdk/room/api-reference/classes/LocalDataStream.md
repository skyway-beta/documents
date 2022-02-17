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

LocalStreamBase.mute

___

### unmute

▸ **unmute**(): `void`

#### Returns

`void`

#### Inherited from

LocalStreamBase.unmute

___

### write

▸ **write**(`object`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `object` | `Object` |

#### Returns

`void`
