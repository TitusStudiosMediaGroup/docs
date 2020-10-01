# Table of Contents

* [angle](e2-docs-angle)
* [array](e2-docs-array)
* [bitwise](e2-docs-bitwise)
* [bone](e2-docs-bone)
* [chat](e2-docs-chat)
* [color](e2-docs-color)
* [compat](e2-docs-compat)
* [complex](e2-docs-complex)
* [console](e2-docs-console)
* [constraint](e2-docs-constraint)
* [core](e2-docs-core)
* [datasignal](e2-docs-datasignal)
* [debug](e2-docs-debug)
* [egpfunctions](e2-docs-egpfunctions)
* [entity](e2-docs-entity)
* [files](e2-docs-files)
* [find](e2-docs-find)
* [gametick](e2-docs-gametick)
* [globalvars](e2-docs-globalvars)
* [hologram](e2-docs-hologram)
* [http](e2-docs-http)
* [matrix](e2-docs-matrix)
* [npc](e2-docs-npc)
* [number](e2-docs-number)
* [player](e2-docs-player)
* [quaternion](e2-docs-quaternion)
* [ranger](e2-docs-ranger)
* [selfaware](e2-docs-selfaware)
* [serialization](e2-docs-serialization)
* [serverinfo](e2-docs-serverinfo)
* [signal](e2-docs-signal)
* [sound](e2-docs-sound)
* [steamidconv](e2-docs-steamidconv)
* [string](e2-docs-string)
* [table](e2-docs-table)
* [timer](e2-docs-timer)
* [unitconv](e2-docs-unitconv)
* [vector](e2-docs-vector)
* [vector2](e2-docs-vector2)
* [weapon](e2-docs-weapon)
* [wirelink](e2-docs-wirelink)
* [custom/camera](e2-docs-custom-camera) (Wire Extras)
* [custom/constraintcore](e2-docs-custom-constraintcore)
* [custom/effects](e2-docs-custom-effects)
* [custom/ftrace](e2-docs-custom-ftrace) (Wire Extras)
* [custom/holoanim](e2-docs-custom-holoanim) (Wire Extras)
* [custom/light](e2-docs-custom-light) (Wire Extras)
* [custom/prop](e2-docs-custom-prop)
* [custom/remoteupload](e2-docs-custom-remoteupload)
* [custom/stcontrol](e2-docs-custom-stcontrol) (Wire Extras)
* [custom/tracesystem](e2-docs-custom-tracesystem) (Wire Extras)
* [custom/wiring](e2-docs-custom-wiring)
***

# Debug

### ![Number](Type-Number.png "Number") = playerCanPrint()

Returns whether or not the next print-message will be printed or omitted by antispam (100 ops)

### print(...)

Prints all arguments to the chat area, seperated by a tab. Automatically does toString for you (Can print arrays but not tables). Works just like lua's print (100 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):printDriver(![String](Type-String.png "String") Text)

Posts a string to the chat of Es driver. Returns 1 if the text was printed, 0 if not (100 ops)

### hint(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") Duration)

Displays a hint popup with message S for N seconds (N being clamped between 0.7 and 7) (100 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):hintDriver(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") Duration)

Displays a hint popup to the driver of vehicle E, with message S for N seconds (N being clamped between 0.7 and 7). Same return value as printDriver (100 ops)

### print(![Number](Type-Number.png "Number") Print_type, ![String](Type-String.png "String") Text)

Same as print(S), but can make the text show up in different places. N can be one of the following: _HUD_PRINTCENTER, _HUD_PRINTCONSOLE, _HUD_PRINTNOTIFY, _HUD_PRINTTALK (100 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):printDriver(![Number](Type-Number.png "Number") Print_type, ![String](Type-String.png "String") Text)

Same as EE:printDriver(S), but can make the text show up in different places. N can be one of the following: _HUD_PRINTCENTER, _HUD_PRINTCONSOLE, _HUD_PRINTNOTIFY, _HUD_PRINTTALK (100 ops)

### printTable(![Array](Type-Array.png "Array") Arr)

Prints an array like the lua function PrintTable does, except to the chat area (100 ops)

### printColor(...)

Works like chat.AddText(...). Parameters can be any amount and combination of numbers, strings, player entities, color vectors (both 3D and 4D) (100 ops)

### printColor(![Array](Type-Array.png "Array") Arr)

Like printColor(...), except taking an array containing all the parameters (100 ops)

### printColorC(...)

Works like MsgC. Parameters can be any amount and combination of numbers, strings, player entities, color vectors (both 3D and 4D) (100 ops)

### printColorC(![Array](Type-Array.png "Array") Arr)

Like printColorC(...), except taking an array containing all the parameters (100 ops)

### ![Entity](Type-Entity.png "Entity"):printColorDriver(... This)

Like printColor but prints to the driver of a specified vehicle (100 ops)

### ![Entity](Type-Entity.png "Entity"):printColorDriver(![Array](Type-Array.png "Array") Arr)

Like printColorDriver but takes an array containing all the parameters (100 ops)