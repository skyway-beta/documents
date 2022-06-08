[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Publication

# Interface: Publication<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`LocalStream`](../modules.md#localstream) = [`LocalStream`](../modules.md#localstream) |

## Table of contents

### Properties

- [codecCapabilities](Publication.md#codeccapabilities)
- [contentType](Publication.md#contenttype)
- [encodings](Publication.md#encodings)
- [id](Publication.md#id)
- [metadata](Publication.md#metadata)
- [onMetadataUpdated](Publication.md#onmetadataupdated)
- [onSubscribed](Publication.md#onsubscribed)
- [onSubscriptionChanged](Publication.md#onsubscriptionchanged)
- [onUnpublished](Publication.md#onunpublished)
- [onUnsubscribed](Publication.md#onunsubscribed)
- [origin](Publication.md#origin)
- [publisher](Publication.md#publisher)
- [status](Publication.md#status)
- [stream](Publication.md#stream)
- [subscriptions](Publication.md#subscriptions)

### Methods

- [cancel](Publication.md#cancel)
- [updateEncodings](Publication.md#updateencodings)
- [updateMetadata](Publication.md#updatemetadata)

## Properties

### codecCapabilities

• `Readonly` **codecCapabilities**: [`Codec`](Codec.md)[]

___

### contentType

• `Readonly` **contentType**: [`ContentType`](../modules.md#contenttype)

___

### encodings

• `Readonly` **encodings**: [`EncodingParameters`](EncodingParameters.md)[]

___

### id

• `Readonly` **id**: `string`

___

### metadata

• `Optional` **metadata**: `string`

___

### onMetadataUpdated

• **onMetadataUpdated**: [`Event`](../classes/Event.md)<{ `metadata`: `string`  }\>

___

### onSubscribed

• **onSubscribed**: [`Event`](../classes/Event.md)<[`StreamSubscribedEvent`](StreamSubscribedEvent.md)\>

___

### onSubscriptionChanged

• **onSubscriptionChanged**: [`Event`](../classes/Event.md)<`void`\>

___

### onUnpublished

• **onUnpublished**: [`Event`](../classes/Event.md)<`void`\>

___

### onUnsubscribed

• **onUnsubscribed**: [`Event`](../classes/Event.md)<[`StreamUnsubscribedEvent`](StreamUnsubscribedEvent.md)\>

___

### origin

• `Optional` `Readonly` **origin**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>

___

### publisher

• **publisher**: [`Member`](Member.md)

___

### status

• **status**: [`PublicationStatus`](../modules.md#publicationstatus)

___

### stream

• `Optional` **stream**: `T`

**`description`** {japanese} publishしたstreamの実体。
ローカルで作られたPublicationでなければundefinedとなる

___

### subscriptions

• `Readonly` **subscriptions**: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>[]

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
| `encodings` | [`EncodingParameters`](EncodingParameters.md)[] |

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
