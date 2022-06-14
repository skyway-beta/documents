[@skyway-sdk/room](../README.md) / [Exports](../modules.md) / RoomSubscription

# Interface: RoomSubscription<T\>

## Type parameters

| Name | Type |
| :------ | :------ |
| `T` | extends [`RemoteStream`](../modules.md#remotestream) = [`RemoteStream`](../modules.md#remotestream) |

## Table of contents

### Properties

- [codec](RoomSubscription.md#codec)
- [contentType](RoomSubscription.md#contenttype)
- [id](RoomSubscription.md#id)
- [onCanceled](RoomSubscription.md#oncanceled)
- [onStreamAttached](RoomSubscription.md#onstreamattached)
- [publication](RoomSubscription.md#publication)
- [status](RoomSubscription.md#status)
- [stream](RoomSubscription.md#stream)
- [subscriber](RoomSubscription.md#subscriber)

### Methods

- [cancel](RoomSubscription.md#cancel)

## Properties

### codec

• `Optional` **codec**: [`Codec`](Codec.md)

___

### contentType

• `Readonly` **contentType**: [`ContentType`](../modules.md#contenttype)

___

### id

• `Readonly` **id**: `string`

___

### onCanceled

• `Readonly` **onCanceled**: [`Event`](../classes/Event.md)<`void`\>

___

### onStreamAttached

• `Readonly` **onStreamAttached**: [`Event`](../classes/Event.md)<`void`\>

___

### publication

• `Readonly` **publication**: [`RoomPublication`](RoomPublication.md)<[`LocalStream`](../modules.md#localstream)\>

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

• `Readonly` **subscriber**: [`RemoteRoomMember`](RemoteRoomMember.md)

## Methods

### cancel

▸ **cancel**(): `Promise`<`void`\>

**`description`** {japanese} unsubscribeする

#### Returns

`Promise`<`void`\>
