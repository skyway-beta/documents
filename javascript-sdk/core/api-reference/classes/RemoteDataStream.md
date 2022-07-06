[@skyway-sdk/core](../README.md) / [Exports](../modules.md) / RemoteDataStream

# Class: RemoteDataStream

## Hierarchy

- [`RemoteStreamBase`](RemoteStreamBase.md)

  ↳ **`RemoteDataStream`**

## Table of contents

### Properties

- [\_datachannel](RemoteDataStream.md#_datachannel)
- [codec](RemoteDataStream.md#codec)
- [contentType](RemoteDataStream.md#contenttype)
- [id](RemoteDataStream.md#id)
- [label](RemoteDataStream.md#label)
- [onData](RemoteDataStream.md#ondata)
- [side](RemoteDataStream.md#side)

## Properties

### \_datachannel

• **\_datachannel**: `RTCDataChannel`

___

### codec

• **codec**: [`Codec`](../interfaces/Codec.md)

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[codec](RemoteStreamBase.md#codec)

___

### contentType

• `Readonly` **contentType**: ``"data"``

#### Overrides

[RemoteStreamBase](RemoteStreamBase.md).[contentType](RemoteStreamBase.md#contenttype)

___

### id

• `Readonly` **id**: `string`

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[id](RemoteStreamBase.md#id)

___

### label

• `Readonly` **label**: `string`

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[label](RemoteStreamBase.md#label)

___

### onData

• `Readonly` **onData**: [`Event`](Event.md)<[`DataStreamMessageType`](../modules.md#datastreammessagetype)\>

___

### side

• `Readonly` **side**: ``"remote"``

#### Inherited from

[RemoteStreamBase](RemoteStreamBase.md).[side](RemoteStreamBase.md#side)
