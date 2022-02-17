[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemoteVideoStream

# Class: RemoteVideoStream

## Hierarchy

- `RemoteStreamBase`

  ↳ **`RemoteVideoStream`**

## Implements

- [`PlayableStream`](../interfaces/PlayableStream.md)

## Table of contents

### Constructors

- [constructor](RemoteVideoStream.md#constructor)

### Properties

- [contentType](RemoteVideoStream.md#contenttype)
- [id](RemoteVideoStream.md#id)
- [label](RemoteVideoStream.md#label)
- [side](RemoteVideoStream.md#side)
- [track](RemoteVideoStream.md#track)

### Methods

- [attach](RemoteVideoStream.md#attach)
- [detach](RemoteVideoStream.md#detach)

## Constructors

### constructor

• **new RemoteVideoStream**(`id`, `label`, `track`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `label` | `string` |
| `track` | `MediaStreamTrack` |

#### Overrides

RemoteStreamBase.constructor

## Properties

### contentType

• `Readonly` **contentType**: ``"video"``

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
| `element` | `HTMLVideoElement` |

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
