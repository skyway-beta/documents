[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemotePersonInterface

# Interface: RemotePersonInterface

## Table of contents

### Properties

- [onPublicationSubscribed](RemotePersonInterface.md#onpublicationsubscribed)
- [onPublicationUnsubscribed](RemotePersonInterface.md#onpublicationunsubscribed)

### Methods

- [subscribe](RemotePersonInterface.md#subscribe)
- [unsubscribe](RemotePersonInterface.md#unsubscribe)

## Properties

### onPublicationSubscribed

• `Readonly` **onPublicationSubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemotePerson がPublicationをSubscribeしたとき

___

### onPublicationUnsubscribed

• `Readonly` **onPublicationUnsubscribed**: [`Event`](../classes/Event.md)<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemotePerson がPublicationをUnsubscribeしたとき

## Methods

### subscribe

▸ **subscribe**(`publicationId`): `Promise`<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

**`description`** {japanese} この RemotePerson にPublicationをSubscribeさせる

#### Parameters

| Name | Type |
| :------ | :------ |
| `publicationId` | `string` |

#### Returns

`Promise`<{ `subscription`: [`Subscription`](Subscription.md)<[`RemoteStream`](../modules.md#remotestream)\>  }\>

___

### unsubscribe

▸ **unsubscribe**(`subscriptionId`): `Promise`<`void`\>

**`description`** {japanese} この RemotePerson にPublicationをUnsubscribeさせる

#### Parameters

| Name | Type |
| :------ | :------ |
| `subscriptionId` | `string` |

#### Returns

`Promise`<`void`\>
