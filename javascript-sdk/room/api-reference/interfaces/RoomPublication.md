[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / RoomPublication

# Interface: RoomPublication<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`LocalStream`](../modules.md#localstream) = [`LocalStream`](../modules.md#localstream) |

## Table of contents

### Properties

- [codecCapabilities](RoomPublication.md#codeccapabilities)
- [contentType](RoomPublication.md#contenttype)
- [encodings](RoomPublication.md#encodings)
- [id](RoomPublication.md#id)
- [metadata](RoomPublication.md#metadata)
- [onMetadataUpdated](RoomPublication.md#onmetadataupdated)
- [onSubscribed](RoomPublication.md#onsubscribed)
- [onSubscriptionChanged](RoomPublication.md#onsubscriptionchanged)
- [onUnpublished](RoomPublication.md#onunpublished)
- [onUnsubscribed](RoomPublication.md#onunsubscribed)
- [publisher](RoomPublication.md#publisher)
- [status](RoomPublication.md#status)
- [stream](RoomPublication.md#stream)
- [subscriptions](RoomPublication.md#subscriptions)

### Methods

- [cancel](RoomPublication.md#cancel)
- [updateEncodings](RoomPublication.md#updateencodings)
- [updateMetadata](RoomPublication.md#updatemetadata)

## Properties

### codecCapabilities

• `Readonly` **codecCapabilities**: [`Codec`](Codec.md)[]

___

### contentType

• `Readonly` **contentType**: `ContentType`

___

### encodings

• **encodings**: `EncodingParameters`[]

___

### id

• `Readonly` **id**: `string`

___

### metadata

• `Optional` **metadata**: `string`

___

### onMetadataUpdated

• `Readonly` **onMetadataUpdated**: [`Event`](../classes/Event.md)<{ `metadata`: `string`  }\>

___

### onSubscribed

• `Readonly` **onSubscribed**: [`Event`](../classes/Event.md)<[`StreamSubscribedEvent`](StreamSubscribedEvent.md)\>

___

### onSubscriptionChanged

• `Readonly` **onSubscriptionChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### onUnpublished

• `Readonly` **onUnpublished**: [`Event`](../classes/Event.md)<`void`\>

___

### onUnsubscribed

• `Readonly` **onUnsubscribed**: [`Event`](../classes/Event.md)<[`StreamUnsubscribedEvent`](StreamUnsubscribedEvent.md)\>

___

### publisher

• `Readonly` **publisher**: [`RoomMember`](RoomMember.md)

___

### status

• **status**: [`PublicationStatus`](../modules.md#publicationstatus)

___

### stream

• `Optional` `Readonly` **stream**: `T`

**`description`** {japanese} publishしたstreamの実体。
ローカルで作られたPublicationでなければundefinedとなる

___

### subscriptions

• **subscriptions**: [`RoomSubscription`](RoomSubscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

## Methods

### cancel

▸ **cancel**(): `Promise`<`void`\>

**`description`** {japanese} unpublishする

#### Returns

`Promise`<`void`\>

___

### updateEncodings

▸ **updateEncodings**(`encodings`): `void`

**`description`** {japanese} Video|Audio Streamの場合、encoding設定を更新する

#### Parameters

| Name | Type |
| :------ | :------ |
| `encodings` | `EncodingParameters`[] |

#### Returns

`void`

___

### updateMetadata

▸ **updateMetadata**(`metadata`): `Promise`<`void`\>

**`description`** {japanese} Metadataの更新

#### Parameters

| Name | Type |
| :------ | :------ |
| `metadata` | `string` |

#### Returns

`Promise`<`void`\>
