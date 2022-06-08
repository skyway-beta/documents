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

### Type Aliases

- [ForwardingStatus](modules.md#forwardingstatus)
- [SfuClientPluginOptions](modules.md#sfuclientpluginoptions)

## Type Aliases

### ForwardingStatus

Ƭ **ForwardingStatus**: ``"started"`` \| ``"stopped"``

___

### SfuClientPluginOptions

Ƭ **SfuClientPluginOptions**: `Omit`<[`SfuApiOptions`](interfaces/SfuApiOptions.md), ``"logLevel"``\> & { `endpointTimeout`: `number`  }
