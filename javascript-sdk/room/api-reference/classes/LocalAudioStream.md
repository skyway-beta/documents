[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalAudioStream

# Class: LocalAudioStream

## Hierarchy

- `LocalStreamBase`

  ↳ **`LocalAudioStream`**

## Implements

- `PlayableStream`
- `LocalPlayableStream`

## Table of contents

### Constructors

- [constructor](LocalAudioStream.md#constructor)

### Properties

- [contentType](LocalAudioStream.md#contenttype)
- [id](LocalAudioStream.md#id)
- [label](LocalAudioStream.md#label)
- [side](LocalAudioStream.md#side)
- [track](LocalAudioStream.md#track)

### Methods

- [attach](LocalAudioStream.md#attach)
- [detach](LocalAudioStream.md#detach)
- [release](LocalAudioStream.md#release)
- [replaceTrack](LocalAudioStream.md#replacetrack)

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

___

### release

▸ **release**(): `void`

#### Returns

`void`

#### Implementation of

LocalPlayableStream.release

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

LocalPlayableStream.replaceTrack
