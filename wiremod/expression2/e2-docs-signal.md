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

# Signal

### signalSetGroup(![String](Type-String.png "String") Group)

Sets the E-2's current signal group to S, this is applied during runOnSignal, signalSend, and signalSetOnRemove calls, so call it first (5 ops)

### ![String](Type-String.png "String") = signalGetGroup()

Gets the E-2's current signal group (5 ops)

### runOnSignal(![String](Type-String.png "String") Name, ![Number](Type-Number.png "Number") Scope, ![Number](Type-Number.png "Number") Activate)

If N2 == 0 the chip will no longer run on this signal, otherwise it makes this chip execute when signal S is sent by someone in scope N (5 ops)

### ![Number](Type-Number.png "Number") = signalClk()

Returns 1 if the chip was executed because of any signal, regardless of name, group or scope. Returns 0 otherwise (1 ops)

### ![Number](Type-Number.png "Number") = signalClk(![String](Type-String.png "String") Name)

Returns 1 if the chip was executed because the signal S was sent, regardless of group or scope. Returns 0 otherwise (1 ops)

### ![Number](Type-Number.png "Number") = signalClk(![String](Type-String.png "String") Name, ![Number](Type-Number.png "Number") Scope)

Returns 1 if the chip was executed because the signal S was sent to the scope N, regardless of group. Returns 0 otherwise (1 ops)

### ![Number](Type-Number.png "Number") = signalClk(![String](Type-String.png "String") Group, ![String](Type-String.png "String") Name)

Returns 1 if the chip was executed because the signal S2 was sent in the group S, regardless of scope. Returns 0 otherwise (1 ops)

### ![Number](Type-Number.png "Number") = signalClk(![String](Type-String.png "String") Group, ![String](Type-String.png "String") Name, ![Number](Type-Number.png "Number") Scope)

Returns 1 if the chip was executed because the signal S2 was sent in the group S to the scope N. Returns 0 otherwise (1 ops)

### ![String](Type-String.png "String") = signalName()

Returns the name of the received signal (4 ops)

### ![String](Type-String.png "String") = signalGroup()

Returns the group name of the received signal (4 ops)

### ![Entity](Type-Entity.png "Entity") = signalSender()

Returns the entity of the chip that sent the signal (4 ops)

### ![Number](Type-Number.png "Number") = signalSenderId()

Returns the entity ID of the chip that sent the signal. Useful if the entity doesn't exist anymore (4 ops)

### signalSetOnRemove(![String](Type-String.png "String") Name, ![Number](Type-Number.png "Number") Scope)

Sets the signal that the chip sends when it is removed from the world (10 ops)

### signalClearOnRemove()

Clears the signal that the chip sends when it is removed from the world (10 ops)

### signalSend(![String](Type-String.png "String") Name, ![Number](Type-Number.png "Number") Scope)

Sends signal S to scope N. Additional calls to this function with the same signal will overwrite the old call until the signal is issued (20 ops)

### signalSendDirect(![String](Type-String.png "String") Name, ![Entity](Type-Entity.png "Entity") Receiver)

Sends signal S to the given chip. Multiple calls for different chips do not overwrite each other (10 ops)

### signalSendToPlayer(![String](Type-String.png "String") Name, ![Entity](Type-Entity.png "Entity") Player)

Sends signal S to chips owned by the given player, multiple calls for different players do not overwrite each other (20 ops)