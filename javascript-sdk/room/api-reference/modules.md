# @skyway-sdk/room

## Table of contents

### Classes

- [LocalAudioStream](classes/LocalAudioStream.md)
- [LocalDataStream](classes/LocalDataStream.md)
- [LocalP2PRoomMember](classes/LocalP2PRoomMember.md)
- [LocalSFURoomMember](classes/LocalSFURoomMember.md)
- [LocalVideoStream](classes/LocalVideoStream.md)
- [Logger](classes/Logger.md)
- [RemoteAudioStream](classes/RemoteAudioStream.md)
- [RemoteDataStream](classes/RemoteDataStream.md)
- [RemoteVideoStream](classes/RemoteVideoStream.md)
- [SkyWayAuthToken](classes/SkyWayAuthToken.md)
- [SkyWayContext](classes/SkyWayContext.md)
- [SkyWayRoom](classes/SkyWayRoom.md)

### Interfaces

- [LocalRoomMember](interfaces/LocalRoomMember.md)
- [MemberJoinedEvent](interfaces/MemberJoinedEvent.md)
- [MemberLeftEvent](interfaces/MemberLeftEvent.md)
- [MemberMetadataUpdatedEvent](interfaces/MemberMetadataUpdatedEvent.md)
- [MembershipChangedEvent](interfaces/MembershipChangedEvent.md)
- [P2PRoom](interfaces/P2PRoom.md)
- [PublicationChangedEvent](interfaces/PublicationChangedEvent.md)
- [PublicationMetadataUpdatedEvent](interfaces/PublicationMetadataUpdatedEvent.md)
- [PublicationOptions](interfaces/PublicationOptions.md)
- [RemoteRoomMember](interfaces/RemoteRoomMember.md)
- [Room](interfaces/Room.md)
- [RoomClosedEvent](interfaces/RoomClosedEvent.md)
- [RoomInit](interfaces/RoomInit.md)
- [RoomMember](interfaces/RoomMember.md)
- [RoomMetadataUpdatedEvent](interfaces/RoomMetadataUpdatedEvent.md)
- [RoomPublication](interfaces/RoomPublication.md)
- [RoomSubscription](interfaces/RoomSubscription.md)
- [SfuRoom](interfaces/SfuRoom.md)
- [SfuRoomPublicationOptions](interfaces/SfuRoomPublicationOptions.md)
- [SkyWayConfigOptions](interfaces/SkyWayConfigOptions.md)
- [StreamPublishedEvent](interfaces/StreamPublishedEvent.md)
- [StreamSubscribedEvent](interfaces/StreamSubscribedEvent.md)
- [StreamUnpublishedEvent](interfaces/StreamUnpublishedEvent.md)
- [StreamUnsubscribedEvent](interfaces/StreamUnsubscribedEvent.md)
- [SubscriptionChangedEvent](interfaces/SubscriptionChangedEvent.md)

### Type aliases

- [LocalStream](modules.md#localstream)
- [MemberSide](modules.md#memberside)
- [MemberStatus](modules.md#memberstatus)
- [MemberType](modules.md#membertype)
- [RemoteStream](modules.md#remotestream)
- [RoomMemberStatus](modules.md#roommemberstatus)
- [RoomPublicationStatus](modules.md#roompublicationstatus)
- [RoomStatus](modules.md#roomstatus)
- [RoomSubscriptionStatus](modules.md#roomsubscriptionstatus)
- [RoomType](modules.md#roomtype)
- [TurnPolicy](modules.md#turnpolicy)

### Variables

- [SkyWayMediaDevices](modules.md#skywaymediadevices)
- [roomTypes](modules.md#roomtypes)

### Functions

- [uuidV4](modules.md#uuidv4)

## Type aliases

### LocalStream

Ƭ **LocalStream**: [`LocalAudioStream`](classes/LocalAudioStream.md) \| [`LocalVideoStream`](classes/LocalVideoStream.md) \| [`LocalDataStream`](classes/LocalDataStream.md)

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

### RemoteStream

Ƭ **RemoteStream**: [`RemoteDataStream`](classes/RemoteDataStream.md) \| [`RemoteAudioStream`](classes/RemoteAudioStream.md) \| [`RemoteVideoStream`](classes/RemoteVideoStream.md)

___

### RoomMemberStatus

Ƭ **RoomMemberStatus**: [`MemberStatus`](modules.md#memberstatus)

___

### RoomPublicationStatus

Ƭ **RoomPublicationStatus**: `PublicationStatus`

___

### RoomStatus

Ƭ **RoomStatus**: `ChannelStatus`

___

### RoomSubscriptionStatus

Ƭ **RoomSubscriptionStatus**: `SubscriptionStatus`

___

### RoomType

Ƭ **RoomType**: typeof [`roomTypes`](modules.md#roomtypes)[`number`]

___

### TurnPolicy

Ƭ **TurnPolicy**: ``"enable"`` \| ``"disable"`` \| ``"turnOnly"``

## Variables

### SkyWayMediaDevices

• **SkyWayMediaDevices**: `MediaDevicesImpl`

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
