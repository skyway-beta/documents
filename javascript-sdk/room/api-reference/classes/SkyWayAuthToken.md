[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / SkyWayAuthToken

# Class: SkyWayAuthToken

## Implements

- `AuthToken`

## Table of contents

### Constructors

- [constructor](SkyWayAuthToken.md#constructor)

### Properties

- [exp](SkyWayAuthToken.md#exp)
- [iat](SkyWayAuthToken.md#iat)
- [jti](SkyWayAuthToken.md#jti)
- [scope](SkyWayAuthToken.md#scope)
- [tokenString](SkyWayAuthToken.md#tokenstring)

### Methods

- [encode](SkyWayAuthToken.md#encode)
- [Decode](SkyWayAuthToken.md#decode)

## Constructors

### constructor

• **new SkyWayAuthToken**(`props`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `props` | `AuthToken` |

## Properties

### exp

• **exp**: `number`

seconds

#### Implementation of

AuthToken.exp

___

### iat

• **iat**: `number`

seconds

#### Implementation of

AuthToken.iat

___

### jti

• **jti**: `string`

uuid

#### Implementation of

AuthToken.jti

___

### scope

• **scope**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `app` | `AppScope` |

#### Implementation of

AuthToken.scope

___

### tokenString

• `Optional` **tokenString**: `string`

## Methods

### encode

▸ **encode**(`secret`): `string`

#### Parameters

| Name | Type |
| :------ | :------ |
| `secret` | `string` |

#### Returns

`string`

___

### Decode

▸ `Static` **Decode**(`token`): [`SkyWayAuthToken`](SkyWayAuthToken.md)

#### Parameters

| Name | Type |
| :------ | :------ |
| `token` | `string` |

#### Returns

[`SkyWayAuthToken`](SkyWayAuthToken.md)
