[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Event

# Class: Event<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `any` |

## Table of contents

### Constructors

- [constructor](Event.md#constructor)

### Properties

- [add](Event.md#add)
- [asPromise](Event.md#aspromise)
- [emit](Event.md#emit)
- [once](Event.md#once)
- [pipe](Event.md#pipe)
- [removeAllListeners](Event.md#removealllisteners)
- [watch](Event.md#watch)

### Accessors

- [length](Event.md#length)

## Constructors

### constructor

• **new Event**<`T`\>(`_onSetListener?`)

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends `unknown` |

#### Parameters

| Name | Type |
| :------ | :------ |
| `_onSetListener?` | () => `void` |

## Properties

### add

• **add**: (`callback`: (`args`: `T`) => `void`) => { `removeListener`: () => `void`  }

#### Type declaration

▸ (`callback`): `Object`

イベントが起きた時に実行する関数を登録する。
戻り値として関数の登録を解除する関数が帰ってくる

##### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`args`: `T`) => `void` |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `removeListener` | () => `void` |

___

### asPromise

• **asPromise**: (`timeLimit?`: `number`) => `Promise`<`T`\>

#### Type declaration

▸ (`timeLimit?`): `Promise`<`T`\>

イベントが起きた時に Promise が resolve される

##### Parameters

| Name | Type | Description |
| :------ | :------ | :------ |
| `timeLimit?` | `number` | ms |

##### Returns

`Promise`<`T`\>

___

### emit

• **emit**: (`arg`: `T`) => `void`

#### Type declaration

▸ (`arg`): `void`

##### Parameters

| Name | Type |
| :------ | :------ |
| `arg` | `T` |

##### Returns

`void`

___

### once

• **once**: (`callback`: (`arg`: `T`) => `void`) => `void`

#### Type declaration

▸ (`callback`): `void`

イベントが起きた時に一度だけ実行される関数を登録する

##### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`arg`: `T`) => `void` |

##### Returns

`void`

___

### pipe

• **pipe**: (`event`: [`Event`](Event.md)<`T`\>) => { `removeListener`: () => `void`  }

#### Type declaration

▸ (`event`): `Object`

##### Parameters

| Name | Type |
| :------ | :------ |
| `event` | [`Event`](Event.md)<`T`\> |

##### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `removeListener` | () => `void` |

___

### removeAllListeners

• **removeAllListeners**: () => `void`

#### Type declaration

▸ (): `void`

##### Returns

`void`

___

### watch

• **watch**: (`callback`: (`arg`: `T`) => `undefined` \| ``null`` \| `boolean`, `timeLimit?`: `number`) => `Promise`<`T`\>

#### Type declaration

▸ (`callback`, `timeLimit?`): `Promise`<`T`\>

イベントが起きた時に実行される boolean を返す関数を登録する。
登録した関数が true を返した時に Promise が resolve される

##### Parameters

| Name | Type |
| :------ | :------ |
| `callback` | (`arg`: `T`) => `undefined` \| ``null`` \| `boolean` |
| `timeLimit?` | `number` |

##### Returns

`Promise`<`T`\>

## Accessors

### length

• `get` **length**(): `number`

#### Returns

`number`
