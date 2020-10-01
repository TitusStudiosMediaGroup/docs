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

# Console

### ![Number](Type-Number.png "Number") = concmd(![String](Type-String.png "String") Command)

Takes a string and executes it in console. Returns 1 if it succeeded and 0 if it failed.The client must enable this in the console with "wire_expression2_concmd 1". "wire_expression2_concmd_whitelist" allows you to choose which commands can be used.[http://www.wiremod.com/forum/151800-post12.html] (5 ops)

### ![String](Type-String.png "String") = convar(![String](Type-String.png "String") Cvar)

Give a console command such as "name" and it returns the set value (5 ops)

### ![Number](Type-Number.png "Number") = convarnum(![String](Type-String.png "String") Cvar)

Give a console command such as "sbox_godmode" and it returns the set value (5 ops)

### ![Number](Type-Number.png "Number") = maxOfType(![String](Type-String.png "String") Typename)

Returns the maximum allowed of a certain type of entity, i.e. maxOfType("wire_thrusters"). Returns 0 if you enter an invalid parameter (5 ops)

### ![Number](Type-Number.png "Number") = playerDamage()

Returns 1 if player vs player damage is enabled on the server (5 ops)