[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / Subscription

# Interface: Subscription<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`RemoteStream`](../modules.md#remotestream) = [`RemoteStream`](../modules.md#remotestream) |

## Table of contents

### Properties

- [codec](Subscription.md#codec)
- [contentType](Subscription.md#contenttype)
- [id](Subscription.md#id)
- [onCanceled](Subscription.md#oncanceled)
- [onStreamAttached](Subscription.md#onstreamattached)
- [publication](Subscription.md#publication)
- [status](Subscription.md#status)
- [stream](Subscription.md#stream)
- [subscriber](Subscription.md#subscriber)

### Methods

- [cancel](Subscription.md#cancel)

## Properties

### codec

• `Optional` **codec**: [`Codec`](Codec.md)

**`description`** {japanese} Streamのコーデック

___

### contentType

• **contentType**: [`ContentType`](../modules.md#contenttype)

___

### id

• **id**: `string`

___

### onCanceled

• **onCanceled**: [`Event`](../classes/Event.md)<`void`\>

___

### onStreamAttached

• **onStreamAttached**: [`Event`](../classes/Event.md)<`void`\>

___

### publication

• **publication**: [`Publication`](Publication.md)<[`LocalStream`](../modules.md#localstream)\>

___

### status

• **status**: [`SubscriptionStatus`](../modules.md#subscriptionstatus)

___

### stream

• `Optional` **stream**: `T`

**`description`** {japanese} subscribeしているStreamの実体。
ローカルでSubscribeしているSubscriptionでなければundefinedとなる

___

### subscriber

• **subscriber**: [`RemoteMember`](RemoteMember.md)

## Methods

### cancel

▸ **cancel**(): `Promise`<`void`\>

**`description`** {japanese} unsubscribeする

#### Returns

`Promise`<`void`\>
