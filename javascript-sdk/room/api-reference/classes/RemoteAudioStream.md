[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / RemoteAudioStream

# Class: RemoteAudioStream

## Hierarchy

- `RemoteStreamBase`

  ↳ **`RemoteAudioStream`**

## Implements

- `PlayableStream`

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

RemoteStreamBase.codec

___

### contentType

• `Readonly` **contentType**: ``"audio"``

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

### side

• `Readonly` **side**: ``"remote"``

#### Inherited from

RemoteStreamBase.side

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

PlayableStream.attach

___

### detach

▸ **detach**(): `void`

**`description`** {english} Detach the stream from the element.

#### Returns

`void`

#### Implementation of

PlayableStream.detach
