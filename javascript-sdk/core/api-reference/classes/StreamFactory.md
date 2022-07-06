[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / StreamFactory

# Class: StreamFactory

## Table of contents

### Properties

- [onDeviceChange](StreamFactory.md#ondevicechange)

### Methods

- [createCameraVideoStream](StreamFactory.md#createcameravideostream)
- [createDataStream](StreamFactory.md#createdatastream)
- [createMicrophoneAudioAndCameraStream](StreamFactory.md#createmicrophoneaudioandcamerastream)
- [createMicrophoneAudioStream](StreamFactory.md#createmicrophoneaudiostream)
- [enumerateDevices](StreamFactory.md#enumeratedevices)
- [enumerateInputAudioDevices](StreamFactory.md#enumerateinputaudiodevices)
- [enumerateInputVideoDevices](StreamFactory.md#enumerateinputvideodevices)
- [enumerateOutputAudioDevices](StreamFactory.md#enumerateoutputaudiodevices)

## Properties

### onDeviceChange

• `Readonly` **onDeviceChange**: [`Event`](Event.md)<{ `device`: [`MediaDevice`](MediaDevice.md) ; `state`: ``"added"`` \| ``"removed"``  }\>

**`description`** {japanese} 一度参照した種類のデバイスの状態が変化した時に発火するイベント

## Methods

### createCameraVideoStream

▸ **createCameraVideoStream**(`options?`): `Promise`<[`LocalVideoStream`](LocalVideoStream.md)\>

**`description`** {japanese} CameraのVideoStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`VideoMediaTrackConstraints`](../modules.md#videomediatrackconstraints) |

#### Returns

`Promise`<[`LocalVideoStream`](LocalVideoStream.md)\>

___

### createDataStream

▸ **createDataStream**(`options?`): `Promise`<[`LocalDataStream`](LocalDataStream.md)\>

**`description`** {japanese} DataStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`DataStreamOptions`](../interfaces/DataStreamOptions.md) |

#### Returns

`Promise`<[`LocalDataStream`](LocalDataStream.md)\>

___

### createMicrophoneAudioAndCameraStream

▸ **createMicrophoneAudioAndCameraStream**(`__namedParameters?`): `Promise`<{ `audio`: [`LocalAudioStream`](LocalAudioStream.md) ; `video`: [`LocalVideoStream`](LocalVideoStream.md)  }\>

**`description`** {japanese} CameraのVideoStreamとマイクのAudioStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters` | `Object` |
| `__namedParameters.audio?` | [`AudioMediaTrackConstraints`](../modules.md#audiomediatrackconstraints) |
| `__namedParameters.video?` | [`VideoMediaTrackConstraints`](../modules.md#videomediatrackconstraints) |

#### Returns

`Promise`<{ `audio`: [`LocalAudioStream`](LocalAudioStream.md) ; `video`: [`LocalVideoStream`](LocalVideoStream.md)  }\>

___

### createMicrophoneAudioStream

▸ **createMicrophoneAudioStream**(`options?`): `Promise`<[`LocalAudioStream`](LocalAudioStream.md)\>

**`description`** {japanese} マイクのAudioStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | [`AudioMediaTrackConstraints`](../modules.md#audiomediatrackconstraints) |

#### Returns

`Promise`<[`LocalAudioStream`](LocalAudioStream.md)\>

___

### enumerateDevices

▸ **enumerateDevices**(): `Promise`<[`MediaDevice`](MediaDevice.md)[]\>

**`description`** {japanese} デバイスの一覧を取得する

#### Returns

`Promise`<[`MediaDevice`](MediaDevice.md)[]\>

___

### enumerateInputAudioDevices

▸ **enumerateInputAudioDevices**(): `Promise`<[`MediaDevice`](MediaDevice.md)[]\>

**`description`** {japanese} 音声入力デバイスの一覧を取得する

#### Returns

`Promise`<[`MediaDevice`](MediaDevice.md)[]\>

___

### enumerateInputVideoDevices

▸ **enumerateInputVideoDevices**(): `Promise`<[`MediaDevice`](MediaDevice.md)[]\>

**`description`** {japanese} 映像入力デバイスの一覧を取得する

#### Returns

`Promise`<[`MediaDevice`](MediaDevice.md)[]\>

___

### enumerateOutputAudioDevices

▸ **enumerateOutputAudioDevices**(): `Promise`<[`MediaDevice`](MediaDevice.md)[]\>

**`description`** {japanese} 音声出力デバイスの一覧を取得する

#### Returns

`Promise`<[`MediaDevice`](MediaDevice.md)[]\>
