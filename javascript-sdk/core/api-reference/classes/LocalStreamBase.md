[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / LocalStreamBase

# Class: LocalStreamBase

## Hierarchy

- **`LocalStreamBase`**

  ↳ [`LocalAudioStream`](LocalAudioStream.md)

  ↳ [`LocalDataStream`](LocalDataStream.md)

  ↳ [`LocalVideoStream`](LocalVideoStream.md)

## Implements

- [`Stream`](../interfaces/Stream.md)

## Table of contents

### Properties

- [contentType](LocalStreamBase.md#contenttype)
- [id](LocalStreamBase.md#id)
- [label](LocalStreamBase.md#label)
- [side](LocalStreamBase.md#side)

### Accessors

- [muted](LocalStreamBase.md#muted)

### Methods

- [mute](LocalStreamBase.md#mute)
- [unmute](LocalStreamBase.md#unmute)

## Properties

### contentType

• `Readonly` **contentType**: [`ContentType`](../modules.md#contenttype)

#### Implementation of

[Stream](../interfaces/Stream.md).[contentType](../interfaces/Stream.md#contenttype)

___

### id

• `Readonly` **id**: `string`

#### Implementation of

[Stream](../interfaces/Stream.md).[id](../interfaces/Stream.md#id)

___

### label

• `Readonly` **label**: `string`

#### Implementation of

[Stream](../interfaces/Stream.md).[label](../interfaces/Stream.md#label)

___

### side

• `Readonly` **side**: ``"local"``

#### Implementation of

[Stream](../interfaces/Stream.md).[side](../interfaces/Stream.md#side)

## Accessors

### muted

• `get` **muted**(): `boolean`

#### Returns

`boolean`

## Methods

### mute

▸ **mute**(): `void`

#### Returns

`void`

___

### unmute

▸ **unmute**(): `void`

#### Returns

`void`
