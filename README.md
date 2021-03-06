<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

-   [discoverBrains][1]
-   [NeeoBrain][2]
    -   [name][3]
    -   [host][4]
    -   [port][5]
    -   [apiVersion][6]
    -   [getSystemInfo][7]
    -   [blink][8]
    -   [getRooms][9]
    -   [getRecipes][10]
    -   [getActiveRecipes][11]
    -   [setForwardActions][12]
    -   [deleteForwardActions][13]
-   [Room][14]
    -   [brain][15]
    -   [name][16]
    -   [key][17]
    -   [deviceCount][18]
    -   [devices][19]
    -   [getDevice][20]
-   [Device][21]
    -   [brain][22]
    -   [name][23]
    -   [roomName][24]
    -   [type][25]
    -   [manufacturer][26]
    -   [key][27]
    -   [macros][28]
    -   [getMacro][29]
-   [Macro][30]
    -   [brain][31]
    -   [name][32]
    -   [key][33]
    -   [label][34]
    -   [deviceName][35]
    -   [deviceKey][36]
    -   [roomName][37]
    -   [roomKey][38]
    -   [trigger][39]
-   [Recipe][40]
    -   [brain][41]
    -   [key][42]
    -   [name][43]
    -   [roomKey][44]
    -   [roomName][45]
    -   [devices][46]
    -   [getDevice][47]
    -   [powerOn][48]
    -   [powerOff][49]

## discoverBrains

Find all brains connected to the local network

Returns **[Array][50]&lt;[NeeoBrain][51]>** All discovered brains on the local network

## NeeoBrain

Class representing a NEEO Brain.

### name

The brain name

Type: [string][52]

### host

The brain host

Type: [string][52]

### port

The brain port

Type: [number][53]

### apiVersion

The brain API version

Type: [string][52]

### getSystemInfo

Get system info.

Returns **[Promise][54]** 

### blink

Make the LED blink

Returns **[Promise][54]** 

### getRooms

Get all rooms

Returns **[Promise][54]&lt;[Array][50]&lt;[Room][55]>>** 

### getRecipes

Get all recipes

Returns **[Promise][54]&lt;[Array][50]&lt;[Recipe][56]>>** 

### getActiveRecipes

Get all active recipes

Returns **[Promise][54]&lt;[Array][50]&lt;[Recipe][56]>>** 

### setForwardActions

Set the forward actions endpoint config

**Parameters**

-   `options` **[Object][57]** The forward actions options
    -   `options.host` **[string][52]** The forward actions server host
    -   `options.port` **[string][52]** The forward actions server port
    -   `options.path` **[string][52]** The forward actions server path (optional, default `'/neeo'`)

Returns **[Promise][54]** 

### deleteForwardActions

Delete the forward actions endpoint config

Returns **[Promise][54]** 

## Room

Class representing a NEEO Recipe.

### brain

The brain this room belongs to

Type: [NeeoBrain][51]

### name

The room name

Type: [string][52]

### key

The room key

Type: [string][52]

### deviceCount

The number of devices assigned to this room

Type: [number][53]

### devices

The devices assigned to this room

Type: [Array][50]&lt;[Device][58]>

### getDevice

Get a device that belongs to this room

**Parameters**

-   `name` **[string][52]** The name of the device to get

Returns **[Device][58]** The matched device

## Device

Class representing a NEEO Device.

### brain

The brain this device belongs to

Type: [NeeoBrain][51]

### name

The name of the device

Type: [string][52]

### roomName

The name of the room this device is assigned to

Type: [string][52]

### type

The device type

Type: [string][52]

### manufacturer

The device manufacturer name

Type: [string][52]

### key

The device key

Type: [string][52]

### macros

The macros for this device

Type: [Array][50]&lt;[Macro][59]>

### getMacro

Get a macro that belongs to this device

**Parameters**

-   `name` **[string][52]** The name of the macro to get

Returns **[Macro][59]** 

## Macro

Class representing a NEEO Device Macro.

### brain

The brain this macro belongs to

Type: [NeeoBrain][51]

### name

The macro name

Type: [string][52]

### key

The macro key

Type: [string][52]

### label

The macro label

Type: [string][52]

### deviceName

The device name this macro belongs to

Type: [string][52]

### deviceKey

The device key this macro belongs to

Type: [string][52]

### roomName

The room name this macro belongs to

Type: [string][52]

### roomKey

The room key this macro belongs to

Type: [string][52]

### trigger

Trigger this macro on the brain

Returns **[Promise][54]** 

## Recipe

Class representing a NEEO Recipe.

### brain

The brain this recipe belongs to

Type: [NeeoBrain][51]

### key

The recipe key

Type: [string][52]

### name

The recipe name

Type: [string][52]

### roomKey

The room key this recipe belongs to

Type: [string][52]

### roomName

The room name this recipe belongs to

Type: [string][52]

### devices

The devices in this recipe

Type: [Array][50]&lt;[Device][58]>

### getDevice

Get a device that belongs to this recipe

**Parameters**

-   `name` **[string][52]** The name of the device to get

Returns **[Device][58]** The matched device

### powerOn

Power on the recipe

Returns **[Promise][54]** 

### powerOff

Power off the recipe

Returns **[Promise][54]** 

[1]: #discoverbrains

[2]: #neeobrain

[3]: #name

[4]: #host

[5]: #port

[6]: #apiversion

[7]: #getsysteminfo

[8]: #blink

[9]: #getrooms

[10]: #getrecipes

[11]: #getactiverecipes

[12]: #setforwardactions

[13]: #deleteforwardactions

[14]: #room

[15]: #brain

[16]: #name-1

[17]: #key

[18]: #devicecount

[19]: #devices

[20]: #getdevice

[21]: #device

[22]: #brain-1

[23]: #name-2

[24]: #roomname

[25]: #type

[26]: #manufacturer

[27]: #key-1

[28]: #macros

[29]: #getmacro

[30]: #macro

[31]: #brain-2

[32]: #name-3

[33]: #key-2

[34]: #label

[35]: #devicename

[36]: #devicekey

[37]: #roomname-1

[38]: #roomkey

[39]: #trigger

[40]: #recipe

[41]: #brain-3

[42]: #key-3

[43]: #name-4

[44]: #roomkey-1

[45]: #roomname-2

[46]: #devices-1

[47]: #getdevice-1

[48]: #poweron

[49]: #poweroff

[50]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array

[51]: #neeobrain

[52]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[53]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[54]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Promise

[55]: #room

[56]: #recipe

[57]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[58]: #device

[59]: #macro
