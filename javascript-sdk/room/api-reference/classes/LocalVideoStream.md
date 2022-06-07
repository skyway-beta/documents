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

### Accessors

- [muted](LocalVideoStream.md#muted)

### Methods

- [attach](LocalVideoStream.md#attach)
- [detach](LocalVideoStream.md#detach)
- [mute](LocalVideoStream.md#mute)
- [replaceTrack](LocalVideoStream.md#replacetrack)
- [unmute](LocalVideoStream.md#unmute)

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
