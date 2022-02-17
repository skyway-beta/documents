[@skyway-sdk/sfu-client](../README.md) / [Exports](../modules.md) / Forwarding

# Class: Forwarding

## Table of contents

### Constructors

- [constructor](Forwarding.md#constructor)

### Properties

- [configure](Forwarding.md#configure)
- [id](Forwarding.md#id)
- [onStopped](Forwarding.md#onstopped)
- [originPublication](Forwarding.md#originpublication)
- [relayingPublication](Forwarding.md#relayingpublication)
- [state](Forwarding.md#state)

### Methods

- [stop](Forwarding.md#stop)

## Constructors

### constructor

• **new Forwarding**(`id`, `configure`, `originPublication`, `relayingPublication`)

#### Parameters

| Name | Type |
| :------ | :------ |
| `id` | `string` |
| `configure` | [`ForwardingConfigure`](../interfaces/ForwardingConfigure.md) |
| `originPublication` | `Publication`<`LocalStream`\> |
| `relayingPublication` | `Publication`<`LocalStream`\> |

## Properties

### configure

• `Readonly` **configure**: [`ForwardingConfigure`](../interfaces/ForwardingConfigure.md)

___

### id

• `Readonly` **id**: `string`

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

### state

• **state**: [`ForwardingState`](../modules.md#forwardingstate) = `'started'`

## Methods

### stop

▸ **stop**(): `void`

#### Returns

`void`
