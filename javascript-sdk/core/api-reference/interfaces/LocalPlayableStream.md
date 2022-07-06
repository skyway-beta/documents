[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / LocalPlayableStream

# Interface: LocalPlayableStream

## Implemented by

- [`LocalAudioStream`](../classes/LocalAudioStream.md)
- [`LocalVideoStream`](../classes/LocalVideoStream.md)

## Table of contents

### Methods

- [release](LocalPlayableStream.md#release)
- [replaceTrack](LocalPlayableStream.md#replacetrack)

## Methods

### release

▸ **release**(): `void`

**`description`** {japanese} Streamを解放します。
カメラやマイクなどのデバイスを解放するためにはそのデバイスに関連するすべてのStreamを解放する必要があります

#### Returns

`void`

___

### replaceTrack

▸ **replaceTrack**(`track`): `void`

**`description`** {japanese} Video|Audio Streamの場合、trackを入れ替える

#### Parameters

| Name | Type |
| :------ | :------ |
| `track` | `MediaStreamTrack` |

#### Returns

`void`
