[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / LocalVideoStream

# Class: LocalVideoStream

## Hierarchy

- `LocalStreamBase`

  ↳ **`LocalVideoStream`**

## Implements

- `PlayableStream`
- `LocalPlayableStream`

## Table of contents

### Constructors

- [constructor](LocalVideoStream.md#constructor)

### Properties

- [contentType](LocalVideoStream.md#contenttype)
- [id](LocalVideoStream.md#id)
- [label](LocalVideoStream.md#label)
- [side](LocalVideoStream.md#side)
- [track](LocalVideoStream.md#track)

### Methods

- [attach](LocalVideoStream.md#attach)
- [detach](LocalVideoStream.md#detach)
- [release](LocalVideoStream.md#release)
- [replaceTrack](LocalVideoStream.md#replacetrack)

## Constructors

### constructor

• **new LocalVideoStream**(`label`, `track`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `label` | `string` |
| `track` | `MediaStreamTrack` |

#### Overrides

LocalStreamBase.constructor

## Properties

### contentType

• `Readonly` **contentType**: ``"video"``

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
| `element` | `HTMLVideoElement` |

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
