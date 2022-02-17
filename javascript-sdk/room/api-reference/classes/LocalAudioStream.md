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

### mute

▸ **mute**(): `void`

#### Returns

`void`

#### Inherited from

LocalStreamBase.mute

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

___

### unmute

▸ **unmute**(): `void`

#### Returns

`void`

#### Inherited from

LocalStreamBase.unmute
