# @skyway-sdk/core

## Table of contents

### Classes

- [Event](classes/Event.md)
- [Events](classes/Events.md)
- [LocalAudioStream](classes/LocalAudioStream.md)
- [LocalDataStream](classes/LocalDataStream.md)
- [LocalVideoStream](classes/LocalVideoStream.md)
- [Logger](classes/Logger.md)
- [MediaDevice](classes/MediaDevice.md)
- [MediaDeviceManager](classes/MediaDeviceManager.md)
- [P2PConnection](classes/P2PConnection.md)
- [RemoteAudioStream](classes/RemoteAudioStream.md)
- [RemoteDataStream](classes/RemoteDataStream.md)
- [RemoteVideoStream](classes/RemoteVideoStream.md)
- [SkyWayAuthToken](classes/SkyWayAuthToken.md)
- [SkyWayChannel](classes/SkyWayChannel.md)
- [SkyWayConfig](classes/SkyWayConfig.md)
- [SkyWayContext](classes/SkyWayContext.md)
- [SkyWayError](classes/SkyWayError.md)

### Interfaces

- [AppScope](interfaces/AppScope.md)
- [AuthToken](interfaces/AuthToken.md)
- [Channel](interfaces/Channel.md)
- [ChannelClosedEvent](interfaces/ChannelClosedEvent.md)
- [ChannelInit](interfaces/ChannelInit.md)
- [ChannelMetadataUpdatedEvent](interfaces/ChannelMetadataUpdatedEvent.md)
- [ChannelQuery](interfaces/ChannelQuery.md)
- [ChannelScope](interfaces/ChannelScope.md)
- [Codec](interfaces/Codec.md)
- [DataStreamOptions](interfaces/DataStreamOptions.md)
- [EncodingParameters](interfaces/EncodingParameters.md)
- [LocalPerson](interfaces/LocalPerson.md)
- [LocalPlayableStream](interfaces/LocalPlayableStream.md)
- [Member](interfaces/Member.md)
- [MemberInit](interfaces/MemberInit.md)
- [MemberJoinedEvent](interfaces/MemberJoinedEvent.md)
- [MemberLeftEvent](interfaces/MemberLeftEvent.md)
- [MemberMetadataUpdatedEvent](interfaces/MemberMetadataUpdatedEvent.md)
- [MemberScope](interfaces/MemberScope.md)
- [MembershipChangedEvent](interfaces/MembershipChangedEvent.md)
- [PlayableStream](interfaces/PlayableStream.md)
- [Publication](interfaces/Publication.md)
- [PublicationChangedEvent](interfaces/PublicationChangedEvent.md)
- [PublicationMetadataUpdatedEvent](interfaces/PublicationMetadataUpdatedEvent.md)
- [PublicationOptions](interfaces/PublicationOptions.md)
- [PublicationScope](interfaces/PublicationScope.md)
- [RemoteMember](interfaces/RemoteMember.md)
- [RtcRpcApiConfig](interfaces/RtcRpcApiConfig.md)
- [SignalEvent](interfaces/SignalEvent.md)
- [SkyWayConfigOptions](interfaces/SkyWayConfigOptions.md)
- [SkyWayConnection](interfaces/SkyWayConnection.md)
- [Stream](interfaces/Stream.md)
- [StreamPublishedEvent](interfaces/StreamPublishedEvent.md)
- [StreamSubscribedEvent](interfaces/StreamSubscribedEvent.md)
- [StreamUnpublishedEvent](interfaces/StreamUnpublishedEvent.md)
- [StreamUnsubscribedEvent](interfaces/StreamUnsubscribedEvent.md)
- [Subscription](interfaces/Subscription.md)
- [SubscriptionChangedEvent](interfaces/SubscriptionChangedEvent.md)
- [SubscriptionScope](interfaces/SubscriptionScope.md)

### Type Aliases

- [AppAction](modules.md#appaction)
- [AudioMediaTrackConstraints](modules.md#audiomediatrackconstraints)
- [ChannelAction](modules.md#channelaction)
- [ChannelStatus](modules.md#channelstatus)
- [ContentType](modules.md#contenttype)
- [DataType](modules.md#datatype)
- [HttpResponse](modules.md#httpresponse)
- [LocalStream](modules.md#localstream)
- [LogLevel](modules.md#loglevel)
- [MemberAction](modules.md#memberaction)
- [MemberSide](modules.md#memberside)
- [MemberStatus](modules.md#memberstatus)
- [MemberType](modules.md#membertype)
- [PublicationAction](modules.md#publicationaction)
- [PublicationStatus](modules.md#publicationstatus)
- [RemotePerson](modules.md#remoteperson)
- [RemoteStream](modules.md#remotestream)
- [RtcApiConfig](modules.md#rtcapiconfig)
- [StreamSide](modules.md#streamside)
- [SubscriptionAction](modules.md#subscriptionaction)
- [SubscriptionStatus](modules.md#subscriptionstatus)
- [TurnCredential](modules.md#turncredential)
- [TurnPolicy](modules.md#turnpolicy)
- [VideoMediaTrackConstraints](modules.md#videomediatrackconstraints)

### Variables

- [SkyWayMediaDevices](modules.md#skywaymediadevices)
- [logLevelTypes](modules.md#logleveltypes)

### Functions

- [uuidV4](modules.md#uuidv4)

## Type Aliases

### AppAction

Ƭ **AppAction**: ``"listChannels"`` \| ``"read"`` \| ``"write"``

___

### AudioMediaTrackConstraints

Ƭ **AudioMediaTrackConstraints**: `Omit`<`MediaTrackConstraints`, ``"aspectRatio"`` \| ``"facingMode"`` \| ``"frameRate"`` \| ``"height"`` \| ``"width"``\>

___

### ChannelAction

Ƭ **ChannelAction**: ``"read"`` \| ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"updateMetadata"``

___

### ChannelStatus

Ƭ **ChannelStatus**: ``"created"`` \| ``"opened"`` \| ``"closed"``

___

### ContentType

Ƭ **ContentType**: ``"audio"`` \| ``"data"`` \| ``"video"``

___

### DataType

Ƭ **DataType**: `string` \| `Blob` \| `ArrayBuffer`

___

### HttpResponse

Ƭ **HttpResponse**: `AxiosResponse` & { `message`: `string`  }

___

### LocalStream

Ƭ **LocalStream**: [`LocalAudioStream`](classes/LocalAudioStream.md) \| [`LocalVideoStream`](classes/LocalVideoStream.md) \| [`LocalDataStream`](classes/LocalDataStream.md)

___

### LogLevel

Ƭ **LogLevel**: typeof [`logLevelTypes`](modules.md#logleveltypes)[`number`]

___

### MemberAction

Ƭ **MemberAction**: ``"create"`` \| ``"write"`` \| ``"delete"`` \| ``"updateMetadata"`` \| ``"signal"``

___

### MemberSide

Ƭ **MemberSide**: ``"local"`` \| ``"remote"``

___

### MemberStatus

Ƭ **MemberStatus**: ``"created"`` \| ``"joined"`` \| ``"left"``

___

### MemberType

Ƭ **MemberType**: ``"person"`` \| ``"bot"``

___

### PublicationAction

Ƭ **PublicationAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"mute"`` \| ``"updateMetadata"`` \| ``"unmute"``

___

### PublicationStatus

Ƭ **PublicationStatus**: ``"created"`` \| ``"published"`` \| ``"canceled"``

___

### RemotePerson

Ƭ **RemotePerson**: [`RemoteMember`](interfaces/RemoteMember.md) & `Person` & `RemotePersonInterface`

___

### RemoteStream

Ƭ **RemoteStream**: [`RemoteDataStream`](classes/RemoteDataStream.md) \| [`RemoteAudioStream`](classes/RemoteAudioStream.md) \| [`RemoteVideoStream`](classes/RemoteVideoStream.md)

___

### RtcApiConfig

Ƭ **RtcApiConfig**: [`RtcRpcApiConfig`](interfaces/RtcRpcApiConfig.md)

___

### StreamSide

Ƭ **StreamSide**: ``"remote"`` \| ``"local"``

___

### SubscriptionAction

Ƭ **SubscriptionAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"unmute"`` \| ``"mute"``

___

### SubscriptionStatus

Ƭ **SubscriptionStatus**: ``"created"`` \| ``"subscribed"`` \| ``"canceled"``

___

### TurnCredential

Ƭ **TurnCredential**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `credential` | `string` |
| `ttl` | `number` |
| `urls` | `string`[] |
| `username` | `string` |

___

### TurnPolicy

Ƭ **TurnPolicy**: ``"enable"`` \| ``"disable"`` \| ``"turnOnly"``

___

### VideoMediaTrackConstraints

Ƭ **VideoMediaTrackConstraints**: `Omit`<`MediaTrackConstraints`, ``"autoGainControl"`` \| ``"channelCount"`` \| ``"echoCancellation"`` \| ``"latency"`` \| ``"noiseSuppression"`` \| ``"sampleRate"`` \| ``"sampleSize"`` \| ``"suppressLocalAudioPlayback"`` \| ``"volume"``\>

## Variables

### SkyWayMediaDevices

• `Const` **SkyWayMediaDevices**: [`MediaDeviceManager`](classes/MediaDeviceManager.md)

___

### logLevelTypes

• `Const` **logLevelTypes**: readonly [``"error"``, ``"warn"``, ``"debug"``, ``"disable"``]

## Functions

### uuidV4

▸ **uuidV4**<`T`\>(`options`, `buffer`, `offset?`): `T`

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `ArrayLike`<`number`, `T`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `options` | `undefined` \| ``null`` \| `V4Options` |
| `buffer` | `T` |
| `offset?` | `number` |

#### Returns

`T`

▸ **uuidV4**(`options?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | `V4Options` |

#### Returns

`string`
