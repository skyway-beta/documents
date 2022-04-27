[@skyway-sdk/token](../README.md) / [Exports](../modules.md) / SkyWayAuthToken

# Class: SkyWayAuthToken

## Implements

- [`AuthToken`](../interfaces/AuthToken.md)

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
| `props` | [`AuthToken`](../interfaces/AuthToken.md) |

## Properties

### exp

• **exp**: `number`

seconds

#### Implementation of

[AuthToken](../interfaces/AuthToken.md).[exp](../interfaces/AuthToken.md#exp)

___

### iat

• **iat**: `number`

seconds

#### Implementation of

[AuthToken](../interfaces/AuthToken.md).[iat](../interfaces/AuthToken.md#iat)

___

### jti

• **jti**: `string`

uuid

#### Implementation of

[AuthToken](../interfaces/AuthToken.md).[jti](../interfaces/AuthToken.md#jti)

___

### scope

• **scope**: `Object`

#### Type declaration

| Name | Type |
| :------ | :------ |
| `app` | [`AppScope`](../interfaces/AppScope.md) |

#### Implementation of

[AuthToken](../interfaces/AuthToken.md).[scope](../interfaces/AuthToken.md#scope)

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
