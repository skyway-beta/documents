# @skyway-sdk/sfu-client

## Table of contents

### Classes

- [Forwarding](classes/Forwarding.md)
- [SFUConnection](classes/SFUConnection.md)
- [SfuBotMember](classes/SfuBotMember.md)
- [SfuClientPlugin](classes/SfuClientPlugin.md)

### Interfaces

- [ForwardingConfigure](interfaces/ForwardingConfigure.md)
- [SfuApiOptions](interfaces/SfuApiOptions.md)

### Type aliases

- [ForwardingState](modules.md#forwardingstate)
- [SfuClientPluginOptions](modules.md#sfuclientpluginoptions)

## Type aliases

### ForwardingState

Ƭ **ForwardingState**: ``"started"`` \| ``"stopped"``

___

### SfuClientPluginOptions

Ƭ **SfuClientPluginOptions**: `Omit`<[`SfuApiOptions`](interfaces/SfuApiOptions.md), ``"logLevel"``\> & { `endpointTimeout`: `number`  }
