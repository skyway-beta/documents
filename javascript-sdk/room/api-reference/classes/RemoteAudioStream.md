[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / RemoteAudioStream

# Class: RemoteAudioStream

## Hierarchy

- `RemoteStreamBase`

  ↳ **`RemoteAudioStream`**

## Implements

- `PlayableStream`

## Table of contents

### Constructors

- [constructor](RemoteAudioStream.md#constructor)

### Properties

- [contentType](RemoteAudioStream.md#contenttype)
- [id](RemoteAudioStream.md#id)
- [label](RemoteAudioStream.md#label)
- [side](RemoteAudioStream.md#side)
- [track](RemoteAudioStream.md#track)

### Methods

- [attach](RemoteAudioStream.md#attach)
- [detach](RemoteAudioStream.md#detach)

## Constructors

### constructor

• **new RemoteAudioStream**(`id`, `label`, `track`)

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
