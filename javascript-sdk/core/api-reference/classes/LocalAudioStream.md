[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / LocalAudioStream

# Class: LocalAudioStream

## Hierarchy

- [`LocalStreamBase`](LocalStreamBase.md)

  ↳ **`LocalAudioStream`**

## Implements

- [`PlayableStream`](../interfaces/PlayableStream.md)
- [`LocalPlayableStream`](../interfaces/LocalPlayableStream.md)

## Table of contents

### Constructors

- [constructor](LocalAudioStream.md#constructor)

### Properties

- [contentType](LocalAudioStream.md#contenttype)
- [id](LocalAudioStream.md#id)
- [label](LocalAudioStream.md#label)
- [side](LocalAudioStream.md#side)
- [track](LocalAudioStream.md#track)

### Accessors

- [muted](LocalAudioStream.md#muted)

### Methods

- [attach](LocalAudioStream.md#attach)
- [detach](LocalAudioStream.md#detach)
- [mute](LocalAudioStream.md#mute)
- [replaceTrack](LocalAudioStream.md#replacetrack)
- [unmute](LocalAudioStream.md#unmute)

## Constructors

### constructor

• **new LocalAudioStream**(`label`, `track`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `label` | `string` |
| `track` | `MediaStreamTrack` |

#### Overrides

LocalStreamBase.constructor

## Properties

### contentType

• `Readonly` **contentType**: ``"audio"``

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

___

### track

• `Readonly` **track**: `MediaStreamTrack`

## Accessors

### muted

• `get` **muted**(): `boolean`

#### Returns

`boolean`

#### Inherited from

LocalStreamBase.muted

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

___

### mute

▸ **mute**(): `void`

#### Returns

`void`

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[mute](LocalStreamBase.md#mute)

___

### replaceTrack

▸ **replaceTrack**(`track`): `void`

#### Parameters

| Name | Type |
| :------ | :------ |
| `track` | `MediaStreamTrack` |

#### Returns

`void`

#### Implementation of

[LocalPlayableStream](../interfaces/LocalPlayableStream.md).[replaceTrack](../interfaces/LocalPlayableStream.md#replacetrack)

___

### unmute

▸ **unmute**(): `void`

#### Returns

`void`

#### Inherited from

[LocalStreamBase](LocalStreamBase.md).[unmute](LocalStreamBase.md#unmute)
