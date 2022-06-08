[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / Forwarding

# Class: Forwarding

## Table of contents

### Properties

- [configure](Forwarding.md#configure)
- [onStopped](Forwarding.md#onstopped)
- [originPublication](Forwarding.md#originpublication)
- [relayingPublication](Forwarding.md#relayingpublication)
- [status](Forwarding.md#status)

### Accessors

- [id](Forwarding.md#id)

### Methods

- [stop](Forwarding.md#stop)
- [toJSON](Forwarding.md#tojson)

## Properties

### configure

• `Readonly` **configure**: [`ForwardingConfigure`](../interfaces/ForwardingConfigure.md)

___

### onStopped

• `Readonly` **onStopped**: `Event`<`void`\>

___

### originPublication

• `Readonly` **originPublication**: `Publication`<`LocalStream`\>

___

### relayingPublication

• `Readonly` **relayingPublication**: `Publication`<`LocalStream`\>

___

### status

• **status**: [`ForwardingStatus`](../modules.md#forwardingstatus) = `'started'`

## Accessors

### id

• `get` **id**(): `string`

#### Returns

`string`

## Methods

### stop

▸ **stop**(): `void`

#### Returns

`void`

___

### toJSON

▸ **toJSON**(): `Object`

#### Returns

`Object`

| Name | Type |
| :------ | :------ |
| `configure` | [`ForwardingConfigure`](../interfaces/ForwardingConfigure.md) |
| `id` | `string` |
| `originPublication` | `Publication`<`LocalStream`\> |
| `relayingPublication` | `Publication`<`LocalStream`\> |
