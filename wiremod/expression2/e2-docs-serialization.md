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

# Serialization

### ![String](Type-String.png "String") = vonEncode(![Array](Type-Array.png "Array") Data)

Encodes an array into a string using vON (10 ops)

### ![String](Type-String.png "String") = vonEncode(![Table](Type-Table.png "Table") Data)

Encodes a table into a string using vON (10 ops)

### ![Array](Type-Array.png "Array") = vonDecode(![String](Type-String.png "String") Data)

Decodes a string into an array using vON (10 ops)

### ![String](Type-String.png "String") = vonError()

Returns the last von error (1 ops)

### ![Table](Type-Table.png "Table") = vonDecodeTable(![String](Type-String.png "String") Data)

Decodes a string into a table using vON (25 ops)

### ![String](Type-String.png "String") = jsonError()

Returns the last json error (1 ops)

### ![String](Type-String.png "String") = jsonEncode(![Table](Type-Table.png "Table") Data)

Encodes a table into a string using json (50 ops)

### ![String](Type-String.png "String") = jsonEncode(![Table](Type-Table.png "Table") Data, ![Number](Type-Number.png "Number") Prettyprint)

Encodes a table into a string using json (50 ops)

### ![Table](Type-Table.png "Table") = jsonDecode(![String](Type-String.png "String") Data)

Decodes a string into an array using json (50 ops)