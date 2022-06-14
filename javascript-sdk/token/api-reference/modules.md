# @skyway-sdk/token

## Table of contents

### Classes

- [SkyWayAuthToken](classes/SkyWayAuthToken.md)

### Interfaces

- [AppScope](interfaces/AppScope.md)
- [AuthToken](interfaces/AuthToken.md)
- [ChannelScope](interfaces/ChannelScope.md)
- [ForwardingScope](interfaces/ForwardingScope.md)
- [MemberScope](interfaces/MemberScope.md)
- [PublicationScope](interfaces/PublicationScope.md)
- [SfuScope](interfaces/SfuScope.md)
- [SfuSubscriptionScope](interfaces/SfuSubscriptionScope.md)
- [SubscriptionScope](interfaces/SubscriptionScope.md)

### Type Aliases

- [AppAction](modules.md#appaction)
- [ChannelAction](modules.md#channelaction)
- [ForwardingAction](modules.md#forwardingaction)
- [MemberAction](modules.md#memberaction)
- [PublicationAction](modules.md#publicationaction)
- [SfuBotAction](modules.md#sfubotaction)
- [SfuSubscriptionAction](modules.md#sfusubscriptionaction)
- [SubscriptionAction](modules.md#subscriptionaction)

### Functions

- [uuidV4](modules.md#uuidv4)

## Type Aliases

### AppAction

Ƭ **AppAction**: ``"listChannels"`` \| ``"read"`` \| ``"write"``

___

### ChannelAction

Ƭ **ChannelAction**: ``"read"`` \| ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"updateMetadata"``

___

### ForwardingAction

Ƭ **ForwardingAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### MemberAction

Ƭ **MemberAction**: ``"create"`` \| ``"write"`` \| ``"delete"`` \| ``"updateMetadata"`` \| ``"signal"``

___

### PublicationAction

Ƭ **PublicationAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"mute"`` \| ``"updateMetadata"`` \| ``"unmute"``

___

### SfuBotAction

Ƭ **SfuBotAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### SfuSubscriptionAction

Ƭ **SfuSubscriptionAction**: ``"create"`` \| ``"write"`` \| ``"delete"``

___

### SubscriptionAction

Ƭ **SubscriptionAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"unmute"`` \| ``"mute"``

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
