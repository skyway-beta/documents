[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / SkyWayRoom

# Class: SkyWayRoom

## Table of contents

### Constructors

- [constructor](SkyWayRoom.md#constructor)

### Methods

- [Create](SkyWayRoom.md#create)
- [Find](SkyWayRoom.md#find)
- [FindOrCreate](SkyWayRoom.md#findorcreate)

## Constructors

### constructor

• **new SkyWayRoom**()

## Methods

### Create

▸ `Static` **Create**<`Init`\>(`context`, `init`): `Promise`<`Init`[``"type"``] extends ``"sfu"`` ? [`SfuRoom`](../interfaces/SfuRoom.md) : [`P2PRoom`](../interfaces/P2PRoom.md)\>

**`description`** {japanese} Roomの作成

#### Type parameters

| Name | Type |
| :------ | :------ |
| `Init` | extends [`RoomInit`](../modules.md#roominit) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `init` | `Init` |

#### Returns

`Promise`<`Init`[``"type"``] extends ``"sfu"`` ? [`SfuRoom`](../interfaces/SfuRoom.md) : [`P2PRoom`](../interfaces/P2PRoom.md)\>

___

### Find

▸ `Static` **Find**<`Type`\>(`context`, `query`, `roomType`, `options?`): `Promise`<`Type` extends ``"sfu"`` ? [`SfuRoom`](../interfaces/SfuRoom.md) : [`P2PRoom`](../interfaces/P2PRoom.md)\>

**`description`** {japanese} 既存のRoomの取得

#### Type parameters

| Name | Type |
| :------ | :------ |
| `Type` | extends ``"sfu"`` \| ``"p2p"`` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `query` | `Object` |
| `query.id?` | `string` |
| `query.name?` | `string` |
| `roomType` | `Type` |
| `options?` | `Type` extends ``"sfu"`` ? [`SfuRoomOptions`](../modules.md#sfuroomoptions) : `void` |

#### Returns

`Promise`<`Type` extends ``"sfu"`` ? [`SfuRoom`](../interfaces/SfuRoom.md) : [`P2PRoom`](../interfaces/P2PRoom.md)\>

___

### FindOrCreate

▸ `Static` **FindOrCreate**<`Init`\>(`context`, `init`): `Promise`<`Init`[``"type"``] extends ``"p2p"`` ? [`P2PRoom`](../interfaces/P2PRoom.md) : [`SfuRoom`](../interfaces/SfuRoom.md)\>

**`description`** {japanese} Roomの取得を試み、存在しなければ作成する

#### Type parameters

| Name | Type |
| :------ | :------ |
| `Init` | extends [`RoomInit`](../modules.md#roominit) |

#### Parameters

| Name | Type |
| :------ | :------ |
| `context` | [`SkyWayContext`](SkyWayContext.md) |
| `init` | `Init` |

#### Returns

`Promise`<`Init`[``"type"``] extends ``"p2p"`` ? [`P2PRoom`](../interfaces/P2PRoom.md) : [`SfuRoom`](../interfaces/SfuRoom.md)\>
