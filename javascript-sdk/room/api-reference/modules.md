# @skyway-sdk/room

## Table of contents

### Classes

- [Event](classes/Event.md)
- [Events](classes/Events.md)
- [LocalAudioStream](classes/LocalAudioStream.md)
- [LocalDataStream](classes/LocalDataStream.md)
- [LocalVideoStream](classes/LocalVideoStream.md)
- [RemoteAudioStream](classes/RemoteAudioStream.md)
- [RemoteDataStream](classes/RemoteDataStream.md)
- [RemoteVideoStream](classes/RemoteVideoStream.md)
- [SkyWayAuthToken](classes/SkyWayAuthToken.md)
- [SkyWayContext](classes/SkyWayContext.md)
- [SkyWayError](classes/SkyWayError.md)
- [SkyWayRoom](classes/SkyWayRoom.md)
- [StreamFactory](classes/StreamFactory.md)

### Interfaces

- [AppScope](interfaces/AppScope.md)
- [AuthToken](interfaces/AuthToken.md)
- [ChannelScope](interfaces/ChannelScope.md)
- [Codec](interfaces/Codec.md)
- [EncodingParameters](interfaces/EncodingParameters.md)
- [ForwardingScope](interfaces/ForwardingScope.md)
- [LocalP2PRoomMember](interfaces/LocalP2PRoomMember.md)
- [LocalRoomMember](interfaces/LocalRoomMember.md)
- [LocalSFURoomMember](interfaces/LocalSFURoomMember.md)
- [MemberJoinedEvent](interfaces/MemberJoinedEvent.md)
- [MemberLeftEvent](interfaces/MemberLeftEvent.md)
- [MemberMetadataUpdatedEvent](interfaces/MemberMetadataUpdatedEvent.md)
- [MemberScope](interfaces/MemberScope.md)
- [MembershipChangedEvent](interfaces/MembershipChangedEvent.md)
- [P2PRoom](interfaces/P2PRoom.md)
- [P2PRoomInit](interfaces/P2PRoomInit.md)
- [PublicationChangedEvent](interfaces/PublicationChangedEvent.md)
- [PublicationMetadataUpdatedEvent](interfaces/PublicationMetadataUpdatedEvent.md)
- [PublicationOptions](interfaces/PublicationOptions.md)
- [PublicationScope](interfaces/PublicationScope.md)
- [RemoteRoomMember](interfaces/RemoteRoomMember.md)
- [Room](interfaces/Room.md)
- [RoomClosedEvent](interfaces/RoomClosedEvent.md)
- [RoomInitBase](interfaces/RoomInitBase.md)
- [RoomMember](interfaces/RoomMember.md)
- [RoomMemberInit](interfaces/RoomMemberInit.md)
- [RoomMetadataUpdatedEvent](interfaces/RoomMetadataUpdatedEvent.md)
- [RoomPublication](interfaces/RoomPublication.md)
- [RoomSubscription](interfaces/RoomSubscription.md)
- [RtcRpcApiConfig](interfaces/RtcRpcApiConfig.md)
- [SfuApiOptions](interfaces/SfuApiOptions.md)
- [SfuRoom](interfaces/SfuRoom.md)
- [SfuRoomInit](interfaces/SfuRoomInit.md)
- [SfuRoomPublicationOptions](interfaces/SfuRoomPublicationOptions.md)
- [SfuScope](interfaces/SfuScope.md)
- [SfuSubscriptionScope](interfaces/SfuSubscriptionScope.md)
- [SkyWayConfigOptions](interfaces/SkyWayConfigOptions.md)
- [StreamPublishedEvent](interfaces/StreamPublishedEvent.md)
- [StreamSubscribedEvent](interfaces/StreamSubscribedEvent.md)
- [StreamUnpublishedEvent](interfaces/StreamUnpublishedEvent.md)
- [StreamUnsubscribedEvent](interfaces/StreamUnsubscribedEvent.md)
- [SubscriptionChangedEvent](interfaces/SubscriptionChangedEvent.md)
- [SubscriptionScope](interfaces/SubscriptionScope.md)

### Type Aliases

- [AppAction](modules.md#appaction)
- [ChannelAction](modules.md#channelaction)
- [ChannelStatus](modules.md#channelstatus)
- [ContentType](modules.md#contenttype)
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
- [RemoteStream](modules.md#remotestream)
- [RoomInit](modules.md#roominit)
- [RoomMemberStatus](modules.md#roommemberstatus)
- [RoomPublicationStatus](modules.md#roompublicationstatus)
- [RoomStatus](modules.md#roomstatus)
- [RoomSubscriptionStatus](modules.md#roomsubscriptionstatus)
- [RoomType](modules.md#roomtype)
- [RtcApiConfig](modules.md#rtcapiconfig)
- [SfuBotAction](modules.md#sfubotaction)
- [SfuClientPluginOptions](modules.md#sfuclientpluginoptions)
- [SfuRoomOptions](modules.md#sfuroomoptions)
- [SfuSubscriptionAction](modules.md#sfusubscriptionaction)
- [SubscriptionAction](modules.md#subscriptionaction)
- [SubscriptionStatus](modules.md#subscriptionstatus)
- [TurnPolicy](modules.md#turnpolicy)

### Variables

- [PACKAGE\_VERSION](modules.md#package_version)
- [SkyWayStreamFactory](modules.md#skywaystreamfactory)
- [logLevelTypes](modules.md#logleveltypes)
- [roomTypes](modules.md#roomtypes)

### Functions

- [uuidV4](modules.md#uuidv4)

## Type Aliases

### AppAction

?? **AppAction**: ``"listChannels"`` \| ``"read"`` \| ``"write"``

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

### RemoteStream

?? **RemoteStream**: [`RemoteDataStream`](classes/RemoteDataStream.md) \| [`RemoteAudioStream`](classes/RemoteAudioStream.md) \| [`RemoteVideoStream`](classes/RemoteVideoStream.md)

___

### RoomInit

?? **RoomInit**: [`P2PRoomInit`](interfaces/P2PRoomInit.md) \| [`SfuRoomInit`](interfaces/SfuRoomInit.md)

___

### RoomMemberStatus

?? **RoomMemberStatus**: [`MemberStatus`](modules.md#memberstatus)

___

### RoomPublicationStatus

?? **RoomPublicationStatus**: [`PublicationStatus`](modules.md#publicationstatus)

___

### RoomStatus

?? **RoomStatus**: [`ChannelStatus`](modules.md#channelstatus)

___

### RoomSubscriptionStatus

?? **RoomSubscriptionStatus**: [`SubscriptionStatus`](modules.md#subscriptionstatus)

___

### RoomType

?? **RoomType**: typeof [`roomTypes`](modules.md#roomtypes)[`number`]

___

### RtcApiConfig

?? **RtcApiConfig**: [`RtcRpcApiConfig`](interfaces/RtcRpcApiConfig.md)

___

### SfuBotAction

?? **SfuBotAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### SfuClientPluginOptions

?? **SfuClientPluginOptions**: `Omit`<[`SfuApiOptions`](interfaces/SfuApiOptions.md), ``"logLevel"``\> & { `endpointTimeout`: `number`  }

___

### SfuRoomOptions

?? **SfuRoomOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `sfu` | `Partial`<[`SfuClientPluginOptions`](modules.md#sfuclientpluginoptions)\> |

___

### SfuSubscriptionAction

?? **SfuSubscriptionAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### SubscriptionAction

?? **SubscriptionAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"unmute"`` \| ``"mute"``

___

### SubscriptionStatus

?? **SubscriptionStatus**: ``"created"`` \| ``"subscribed"`` \| ``"canceled"``

___

### TurnPolicy

?? **TurnPolicy**: ``"enable"`` \| ``"disable"`` \| ``"turnOnly"``

## Variables

### PACKAGE\_VERSION

??? `Const` **PACKAGE\_VERSION**: ``"0.4.0-beta.0"``

___

### SkyWayStreamFactory

??? `Const` **SkyWayStreamFactory**: [`StreamFactory`](classes/StreamFactory.md)

___

### logLevelTypes

??? `Const` **logLevelTypes**: readonly [``"error"``, ``"warn"``, ``"debug"``, ``"disable"``]

___

### roomTypes

??? `Const` **roomTypes**: readonly [``"sfu"``, ``"p2p"``]

## Functions

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
