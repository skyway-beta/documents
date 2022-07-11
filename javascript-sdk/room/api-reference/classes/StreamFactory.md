[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / StreamFactory

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

• `Readonly` **onDeviceChange**: [`Event`](Event.md)<{ `device`: `MediaDevice` ; `state`: ``"added"`` \| ``"removed"``  }\>

**`description`** {japanese} 一度参照した種類のデバイスの状態が変化した時に発火するイベント

## Methods

### createCameraVideoStream

▸ **createCameraVideoStream**(`options?`): `Promise`<[`LocalVideoStream`](LocalVideoStream.md)\>

**`description`** {japanese} CameraのVideoStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | `VideoMediaTrackConstraints` |

#### Returns

`Promise`<[`LocalVideoStream`](LocalVideoStream.md)\>

___

### createDataStream

▸ **createDataStream**(`options?`): `Promise`<[`LocalDataStream`](LocalDataStream.md)\>

**`description`** {japanese} DataStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | `DataStreamOptions` |

#### Returns

`Promise`<[`LocalDataStream`](LocalDataStream.md)\>

___

### createMicrophoneAudioAndCameraStream

▸ **createMicrophoneAudioAndCameraStream**(`__namedParameters?`): `Promise`<{ `audio`: [`LocalAudioStream`](LocalAudioStream.md) ; `video`: [`LocalVideoStream`](LocalVideoStream.md)  }\>

**`description`** {japanese} CameraのVideoStreamとマイクのAudioStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `__namedParameters?` | `Object` |
| `__namedParameters.audio?` | `AudioMediaTrackConstraints` |
| `__namedParameters.video?` | `VideoMediaTrackConstraints` |

#### Returns

`Promise`<{ `audio`: [`LocalAudioStream`](LocalAudioStream.md) ; `video`: [`LocalVideoStream`](LocalVideoStream.md)  }\>

___

### createMicrophoneAudioStream

▸ **createMicrophoneAudioStream**(`options?`): `Promise`<[`LocalAudioStream`](LocalAudioStream.md)\>

**`description`** {japanese} マイクのAudioStreamを作成する

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | `AudioMediaTrackConstraints` |

#### Returns

`Promise`<[`LocalAudioStream`](LocalAudioStream.md)\>

___

### enumerateDevices

▸ **enumerateDevices**(): `Promise`<`MediaDevice`[]\>

**`description`** {japanese} デバイスの一覧を取得する

#### Returns

`Promise`<`MediaDevice`[]\>

___

### enumerateInputAudioDevices

▸ **enumerateInputAudioDevices**(): `Promise`<`MediaDevice`[]\>

**`description`** {japanese} 音声入力デバイスの一覧を取得する

#### Returns

`Promise`<`MediaDevice`[]\>

___

### enumerateInputVideoDevices

▸ **enumerateInputVideoDevices**(): `Promise`<`MediaDevice`[]\>

**`description`** {japanese} 映像入力デバイスの一覧を取得する

#### Returns

`Promise`<`MediaDevice`[]\>

___

### enumerateOutputAudioDevices

▸ **enumerateOutputAudioDevices**(): `Promise`<`MediaDevice`[]\>

**`description`** {japanese} 音声出力デバイスの一覧を取得する

#### Returns

`Promise`<`MediaDevice`[]\>
