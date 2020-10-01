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

# Chat

### runOnChat(![Number](Type-Number.png "Number") Activate)

If set to 0, the chip will no longer run on chat events, otherwise it makes this chip execute when someone chats. Only needs to be called once, not in every execution (3 ops)

### ![Number](Type-Number.png "Number") = chatClk()

Returns 1 if the chip is being executed because of a chat event. Returns 0 otherwise (3 ops)

### ![Number](Type-Number.png "Number") = chatClk(![Entity](Type-Entity.png "Entity") Ply)

Returns 1 if the chip is being executed because of a chat event by player E. Returns 0 otherwise (3 ops)

### hideChat(![Number](Type-Number.png "Number") Hide)

Hides the chat messages written by E2 owner (3 ops)

### ![Entity](Type-Entity.png "Entity") = lastSpoke()

Returns the last player to speak (3 ops)

### ![String](Type-String.png "String") = lastSaid()

Returns the last message in the chat log (3 ops)

### ![Number](Type-Number.png "Number") = lastSaidWhen()

Returns the time the last message was sent (3 ops)

### ![Number](Type-Number.png "Number") = lastSaidTeam()

Returns 1 if the last message was sent in the team chat, 0 otherwise (3 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):lastSaid()

Returns what the player E last said (3 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):lastSaidWhen()

Returns when the given player last said something (3 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):lastSaidTeam()

Returns 1 if the last message was sent in the team chat, 0 otherwise (3 ops)