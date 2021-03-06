# @skyway-sdk/core

## Table of contents

### Classes

- [Event](classes/Event.md)
- [Events](classes/Events.md)
- [LocalAudioStream](classes/LocalAudioStream.md)
- [LocalDataStream](classes/LocalDataStream.md)
- [LocalStreamBase](classes/LocalStreamBase.md)
- [LocalVideoStream](classes/LocalVideoStream.md)
- [MediaDevice](classes/MediaDevice.md)
- [P2PConnection](classes/P2PConnection.md)
- [RemoteAudioStream](classes/RemoteAudioStream.md)
- [RemoteDataStream](classes/RemoteDataStream.md)
- [RemoteStreamBase](classes/RemoteStreamBase.md)
- [RemoteVideoStream](classes/RemoteVideoStream.md)
- [SkyWayAuthToken](classes/SkyWayAuthToken.md)
- [SkyWayChannel](classes/SkyWayChannel.md)
- [SkyWayConfig](classes/SkyWayConfig.md)
- [SkyWayContext](classes/SkyWayContext.md)
- [SkyWayError](classes/SkyWayError.md)
- [StreamFactory](classes/StreamFactory.md)

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
- [ForwardingScope](interfaces/ForwardingScope.md)
- [LocalPerson](interfaces/LocalPerson.md)
- [LocalPlayableStream](interfaces/LocalPlayableStream.md)
- [Member](interfaces/Member.md)
- [MemberInit](interfaces/MemberInit.md)
- [MemberJoinedEvent](interfaces/MemberJoinedEvent.md)
- [MemberLeftEvent](interfaces/MemberLeftEvent.md)
- [MemberMetadataUpdatedEvent](interfaces/MemberMetadataUpdatedEvent.md)
- [MemberScope](interfaces/MemberScope.md)
- [MembershipChangedEvent](interfaces/MembershipChangedEvent.md)
- [Person](interfaces/Person.md)
- [PlayableStream](interfaces/PlayableStream.md)
- [Publication](interfaces/Publication.md)
- [PublicationChangedEvent](interfaces/PublicationChangedEvent.md)
- [PublicationMetadataUpdatedEvent](interfaces/PublicationMetadataUpdatedEvent.md)
- [PublicationOptions](interfaces/PublicationOptions.md)
- [PublicationScope](interfaces/PublicationScope.md)
- [RemoteMember](interfaces/RemoteMember.md)
- [RemotePersonInterface](interfaces/RemotePersonInterface.md)
- [RtcRpcApiConfig](interfaces/RtcRpcApiConfig.md)
- [SfuScope](interfaces/SfuScope.md)
- [SfuSubscriptionScope](interfaces/SfuSubscriptionScope.md)
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
- [DataStreamMessageType](modules.md#datastreammessagetype)
- [DataType](modules.md#datatype)
- [ForwardingAction](modules.md#forwardingaction)
- [HttpResponse](modules.md#httpresponse)
- [LocalStream](modules.md#localstream)
- [LogFormat](modules.md#logformat)
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
- [SfuBotAction](modules.md#sfubotaction)
- [SfuSubscriptionAction](modules.md#sfusubscriptionaction)
- [StreamSide](modules.md#streamside)
- [SubscriptionAction](modules.md#subscriptionaction)
- [SubscriptionStatus](modules.md#subscriptionstatus)
- [TurnCredential](modules.md#turncredential)
- [TurnPolicy](modules.md#turnpolicy)
- [VideoMediaTrackConstraints](modules.md#videomediatrackconstraints)

### Variables

- [SkyWayStreamFactory](modules.md#skywaystreamfactory)
- [logLevelTypes](modules.md#logleveltypes)
- [objectFlag](modules.md#objectflag)

### Functions

- [isSafari](modules.md#issafari)
- [setEncodingParams](modules.md#setencodingparams)
- [uuidV4](modules.md#uuidv4)

## Type Aliases

### AppAction

?? **AppAction**: ``"listChannels"`` \| ``"read"`` \| ``"write"``

___

### AudioMediaTrackConstraints

?? **AudioMediaTrackConstraints**: `Pick`<`MediaTrackConstraintSet`, ``"autoGainControl"`` \| ``"channelCount"`` \| ``"echoCancellation"`` \| ``"latency"`` \| ``"noiseSuppression"`` \| ``"sampleRate"`` \| ``"sampleSize"`` \| ``"suppressLocalAudioPlayback"``\> & { `volume?`: `number`  }

___

### ChannelAction

?? **ChannelAction**: ``"read"`` \| ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"updateMetadata"``

___

### ChannelStatus

?? **ChannelStatus**: ``"created"`` \| ``"opened"`` \| ``"closed"``

___

### ContentType

?? **ContentType**: ``"audio"`` \| ``"data"`` \| ``"video"``

___

### DataStreamMessageType

?? **DataStreamMessageType**: `string` \| `ArrayBuffer` \| `object`

___

### DataType

?? **DataType**: `string` \| `Blob` \| `ArrayBuffer`

___

### ForwardingAction

?? **ForwardingAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### HttpResponse

?? **HttpResponse**: `AxiosResponse` & { `message`: `string`  }

___

### LocalStream

?? **LocalStream**: [`LocalAudioStream`](classes/LocalAudioStream.md) \| [`LocalVideoStream`](classes/LocalVideoStream.md) \| [`LocalDataStream`](classes/LocalDataStream.md)

___

### LogFormat

?? **LogFormat**: ``"object"`` \| ``"string"``

___

### LogLevel

?? **LogLevel**: typeof [`logLevelTypes`](modules.md#logleveltypes)[`number`]

___

### MemberAction

?? **MemberAction**: ``"create"`` \| ``"write"`` \| ``"delete"`` \| ``"updateMetadata"`` \| ``"signal"``

___

### MemberSide

?? **MemberSide**: ``"local"`` \| ``"remote"``

___

### MemberStatus

?? **MemberStatus**: ``"created"`` \| ``"joined"`` \| ``"left"``

___

### MemberType

?? **MemberType**: ``"person"`` \| ``"bot"``

___

### PublicationAction

?? **PublicationAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"mute"`` \| ``"updateMetadata"`` \| ``"unmute"``

___

### PublicationStatus

?? **PublicationStatus**: ``"created"`` \| ``"published"`` \| ``"canceled"``

___

### RemotePerson

?? **RemotePerson**: `RemoteMemberImplInterface` & [`Person`](interfaces/Person.md) & [`RemotePersonInterface`](interfaces/RemotePersonInterface.md)

___

### RemoteStream

?? **RemoteStream**: [`RemoteDataStream`](classes/RemoteDataStream.md) \| [`RemoteAudioStream`](classes/RemoteAudioStream.md) \| [`RemoteVideoStream`](classes/RemoteVideoStream.md)

___

### RtcApiConfig

?? **RtcApiConfig**: [`RtcRpcApiConfig`](interfaces/RtcRpcApiConfig.md)

___

### SfuBotAction

?? **SfuBotAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### SfuSubscriptionAction

?? **SfuSubscriptionAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### StreamSide

?? **StreamSide**: ``"remote"`` \| ``"local"``

___

### SubscriptionAction

?? **SubscriptionAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"unmute"`` \| ``"mute"``

___

### SubscriptionStatus

?? **SubscriptionStatus**: ``"created"`` \| ``"subscribed"`` \| ``"canceled"``

___

### TurnCredential

?? **TurnCredential**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `credential` | `string` |
| `ttl` | `number` |
| `urls` | `string`[] |
| `username` | `string` |

___

### TurnPolicy

?? **TurnPolicy**: ``"enable"`` \| ``"disable"`` \| ``"turnOnly"``

___

### VideoMediaTrackConstraints

?? **VideoMediaTrackConstraints**: `Pick`<`MediaTrackConstraintSet`, ``"aspectRatio"`` \| ``"facingMode"`` \| ``"frameRate"`` \| ``"height"`` \| ``"width"``\>

## Variables

### SkyWayStreamFactory

??? `Const` **SkyWayStreamFactory**: [`StreamFactory`](classes/StreamFactory.md)

___

### logLevelTypes

??? `Const` **logLevelTypes**: readonly [``"error"``, ``"warn"``, ``"debug"``, ``"disable"``]

___

### objectFlag

??? `Const` **objectFlag**: ``"skyway_object:"``

## Functions

### isSafari

??? **isSafari**(): `boolean`

#### Returns

`boolean`

___

### setEncodingParams

??? **setEncodingParams**(`sender`, `newEncodings`): `Promise`<`void`\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `sender` | `RTCRtpSender` |
| `newEncodings` | `RTCRtpEncodingParameters`[] |

#### Returns

`Promise`<`void`\>

___

### uuidV4

??? **uuidV4**<`T`\>(`options`, `buffer`, `offset?`): `T`

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

??? **uuidV4**(`options?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | `V4Options` |

#### Returns

`string`
