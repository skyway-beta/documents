# @skyway-sdk/room

## Table of contents

### Classes

- [Event](classes/Event.md)
- [Events](classes/Events.md)
- [LocalAudioStream](classes/LocalAudioStream.md)
- [LocalDataStream](classes/LocalDataStream.md)
- [LocalVideoStream](classes/LocalVideoStream.md)
- [Logger](classes/Logger.md)
- [MediaDeviceManager](classes/MediaDeviceManager.md)
- [RemoteAudioStream](classes/RemoteAudioStream.md)
- [RemoteDataStream](classes/RemoteDataStream.md)
- [RemoteVideoStream](classes/RemoteVideoStream.md)
- [SkyWayAuthToken](classes/SkyWayAuthToken.md)
- [SkyWayContext](classes/SkyWayContext.md)
- [SkyWayError](classes/SkyWayError.md)
- [SkyWayRoom](classes/SkyWayRoom.md)

### Interfaces

- [AppScope](interfaces/AppScope.md)
- [AuthToken](interfaces/AuthToken.md)
- [ChannelScope](interfaces/ChannelScope.md)
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
- [SkyWayConfigOptions](interfaces/SkyWayConfigOptions.md)
- [StreamPublishedEvent](interfaces/StreamPublishedEvent.md)
- [StreamSubscribedEvent](interfaces/StreamSubscribedEvent.md)
- [StreamUnpublishedEvent](interfaces/StreamUnpublishedEvent.md)
- [StreamUnsubscribedEvent](interfaces/StreamUnsubscribedEvent.md)
- [SubscriptionChangedEvent](interfaces/SubscriptionChangedEvent.md)
- [SubscriptionScope](interfaces/SubscriptionScope.md)

### Type aliases

- [AppAction](modules.md#appaction)
- [ChannelAction](modules.md#channelaction)
- [ChannelStatus](modules.md#channelstatus)
- [HttpResponse](modules.md#httpresponse)
- [LocalStream](modules.md#localstream)
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
- [SfuClientPluginOptions](modules.md#sfuclientpluginoptions)
- [SfuRoomOptions](modules.md#sfuroomoptions)
- [SubscriptionAction](modules.md#subscriptionaction)
- [SubscriptionStatus](modules.md#subscriptionstatus)
- [TurnPolicy](modules.md#turnpolicy)

### Variables

- [SkyWayMediaDevices](modules.md#skywaymediadevices)
- [logLevelTypes](modules.md#logleveltypes)
- [roomTypes](modules.md#roomtypes)

### Functions

- [uuidV4](modules.md#uuidv4)

## Type aliases

### AppAction

Ƭ **AppAction**: ``"listChannels"`` \| ``"read"`` \| ``"write"``

___

### ChannelAction

Ƭ **ChannelAction**: ``"read"`` \| ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"updateMetadata"``

___

### ChannelStatus

Ƭ **ChannelStatus**: ``"created"`` \| ``"opened"`` \| ``"closed"``

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

Ƭ **MemberAction**: ``"create"`` \| ``"write"`` \| ``"delete"`` \| ``"updateMetadata"``

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

Ƭ **PublicationAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"mute"`` \| ``"unmute"``

___

### PublicationStatus

Ƭ **PublicationStatus**: ``"created"`` \| ``"published"`` \| ``"canceled"``

___

### RemoteStream

Ƭ **RemoteStream**: [`RemoteDataStream`](classes/RemoteDataStream.md) \| [`RemoteAudioStream`](classes/RemoteAudioStream.md) \| [`RemoteVideoStream`](classes/RemoteVideoStream.md)

___

### RoomInit

Ƭ **RoomInit**: [`P2PRoomInit`](interfaces/P2PRoomInit.md) \| [`SfuRoomInit`](interfaces/SfuRoomInit.md)

___

### RoomMemberStatus

Ƭ **RoomMemberStatus**: [`MemberStatus`](modules.md#memberstatus)

___

### RoomPublicationStatus

Ƭ **RoomPublicationStatus**: [`PublicationStatus`](modules.md#publicationstatus)

___

### RoomStatus

Ƭ **RoomStatus**: [`ChannelStatus`](modules.md#channelstatus)

___

### RoomSubscriptionStatus

Ƭ **RoomSubscriptionStatus**: [`SubscriptionStatus`](modules.md#subscriptionstatus)

___

### RoomType

Ƭ **RoomType**: typeof [`roomTypes`](modules.md#roomtypes)[`number`]

___

### RtcApiConfig

Ƭ **RtcApiConfig**: [`RtcRpcApiConfig`](interfaces/RtcRpcApiConfig.md)

___

### SfuClientPluginOptions

Ƭ **SfuClientPluginOptions**: `Omit`<[`SfuApiOptions`](interfaces/SfuApiOptions.md), ``"logLevel"``\> & { `endpointTimeout`: `number`  }

___

### SfuRoomOptions

Ƭ **SfuRoomOptions**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `sfu` | `Partial`<[`SfuClientPluginOptions`](modules.md#sfuclientpluginoptions)\> |

___

### SubscriptionAction

Ƭ **SubscriptionAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"unmute"`` \| ``"mute"``

___

### SubscriptionStatus

Ƭ **SubscriptionStatus**: ``"created"`` \| ``"subscribed"`` \| ``"canceled"``

___

### TurnPolicy

Ƭ **TurnPolicy**: ``"enable"`` \| ``"disable"`` \| ``"turnOnly"``

## Variables

### SkyWayMediaDevices

• **SkyWayMediaDevices**: [`MediaDeviceManager`](classes/MediaDeviceManager.md)

___

### logLevelTypes

• **logLevelTypes**: readonly [``"error"``, ``"warn"``, ``"debug"``, ``"disable"``]

___

### roomTypes

• **roomTypes**: readonly [``"sfu"``, ``"p2p"``]

## Functions

### uuidV4

▸ `Const` **uuidV4**<`T`\>(`options`, `buffer`, `offset?`): `T`

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

▸ `Const` **uuidV4**(`options?`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `options?` | `V4Options` |

#### Returns

`string`
