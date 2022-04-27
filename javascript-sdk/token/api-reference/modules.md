# @skyway-sdk/token

## Table of contents

### Classes

- [SkyWayAuthToken](classes/SkyWayAuthToken.md)

### Interfaces

- [AppScope](interfaces/AppScope.md)
- [AuthToken](interfaces/AuthToken.md)
- [ChannelScope](interfaces/ChannelScope.md)
- [MemberScope](interfaces/MemberScope.md)
- [PublicationScope](interfaces/PublicationScope.md)
- [SubscriptionScope](interfaces/SubscriptionScope.md)

### Type aliases

- [AppAction](modules.md#appaction)
- [ChannelAction](modules.md#channelaction)
- [MemberAction](modules.md#memberaction)
- [PublicationAction](modules.md#publicationaction)
- [SubscriptionAction](modules.md#subscriptionaction)

### Functions

- [uuidV4](modules.md#uuidv4)

## Type aliases

### AppAction

Ƭ **AppAction**: ``"listChannels"`` \| ``"read"`` \| ``"write"``

___

### ChannelAction

Ƭ **ChannelAction**: ``"read"`` \| ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"updateMetadata"``

___

### MemberAction

Ƭ **MemberAction**: ``"create"`` \| ``"write"`` \| ``"delete"`` \| ``"updateMetadata"``

___

### PublicationAction

Ƭ **PublicationAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"mute"`` \| ``"unmute"``

___

### SubscriptionAction

Ƭ **SubscriptionAction**: ``"write"`` \| ``"create"`` \| ``"delete"`` \| ``"unmute"`` \| ``"mute"``

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
