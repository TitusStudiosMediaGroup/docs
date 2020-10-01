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

# Serverinfo

### ![String](Type-String.png "String") = map()

Returns the current map name (1 ops)

### ![String](Type-String.png "String") = hostname()

Returns the Name of the server (1 ops)

### ![String](Type-String.png "String") = hostip()

Returns the IP of the server (1 ops)

### ![Number](Type-Number.png "Number") = isLan()

Returns 1 if lan mode is enabled (1 ops)

### ![String](Type-String.png "String") = gamemode()

Returns the name of the current gamemode (1 ops)

### ![String](Type-String.png "String") = serverUUID()

 (1 ops)

### ![Number](Type-Number.png "Number") = isSinglePlayer()

Returns 1 if singleplayer, 0 if multiplayer (1 ops)

### ![Number](Type-Number.png "Number") = isDedicated()

Returns 1 if server is dedicated, 0 if listen (1 ops)

### ![Number](Type-Number.png "Number") = numPlayers()

Returns the number of players currently in the server (1 ops)

### ![Number](Type-Number.png "Number") = maxPlayers()

Returns the max number of players allowed in the server (1 ops)

### ![Number](Type-Number.png "Number") = gravity()

Returns gravity (1 ops)

### ![Vector](Type-Vector.png "Vector") = propGravity()

 (1 ops)

### ![Number](Type-Number.png "Number") = airDensity()

Returns air density (affects how drag slows down props) (1 ops)

### ![Number](Type-Number.png "Number") = maxFrictionMass()

Returns how much friction influences props throughout the server (1 ops)

### ![Number](Type-Number.png "Number") = minFrictionMass()

Returns how much friction influences props throughout the server (1 ops)

### ![Number](Type-Number.png "Number") = speedLimit()

Returns the speed limit (1 ops)

### ![Number](Type-Number.png "Number") = angSpeedLimit()

Returns the angular speed limit (1 ops)

### ![Number](Type-Number.png "Number") = tickInterval()

Returns the time (in seconds) between each server tick (1 ops)