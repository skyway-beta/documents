[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemoteAudioStream

# Class: RemoteAudioStream

## Hierarchy

- [`RemoteStreamBase`](RemoteStreamBase.md)

  ↳ **`RemoteAudioStream`**

## Implements

- [`PlayableStream`](../interfaces/PlayableStream.md)

## Table of contents

### Properties

- [codec](RemoteAudioStream.md#codec)
- [contentType](RemoteAudioStream.md#contenttype)
- [id](RemoteAudioStream.md#id)
- [label](RemoteAudioStream.md#label)
- [side](RemoteAudioStream.md#side)
- [track](RemoteAudioStream.md#track)

### Methods

- [attach](RemoteAudioStream.md#attach)
- [detach](RemoteAudioStream.md#detach)

## Properties

### codec

• **codec**: [`Codec`](../interfaces/Codec.md)

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[codec](RemoteStreamBase.md#codec)

___

### contentType

• `Readonly` **contentType**: ``"audio"``

#### Overrides

[RemoteStreamBase](RemoteStreamBase.md).[contentType](RemoteStreamBase.md#contenttype)

___

### id

• `Readonly` **id**: `string`

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[id](RemoteStreamBase.md#id)

___

### label

• `Readonly` **label**: `string`

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[label](RemoteStreamBase.md#label)

___

### side

• `Readonly` **side**: ``"remote"``

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[side](RemoteStreamBase.md#side)

___

### track

• `Readonly` **track**: `MediaStreamTrack`

## Methods

### attach

▸ **attach**(`element`): `void`

**`description`** {english} Attach the stream to the element.

#### Parameters

| Name | Type |
| :------ | :------ |
| `element` | `HTMLAudioElement` \| `HTMLVideoElement` |

#### Returns

`void`

#### Implementation of

[PlayableStream](../interfaces/PlayableStream.md).[attach](../interfaces/PlayableStream.md#attach)

___

### detach

▸ **detach**(): `void`

**`description`** {english} Detach the stream from the element.

#### Returns

`void`

#### Implementation of

[PlayableStream](../interfaces/PlayableStream.md).[detach](../interfaces/PlayableStream.md#detach)
