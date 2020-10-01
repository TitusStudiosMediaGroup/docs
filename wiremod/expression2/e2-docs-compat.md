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

# Compat

### ![String](Type-String.png "String") = ![Number](Type-Number.png "Number"):teamName()

Returns the name of the team associated with the team number (10 ops)

### ![Number](Type-Number.png "Number") = ![Number](Type-Number.png "Number"):teamScore()

Returns the score of the team associated with the team number (10 ops)

### ![Number](Type-Number.png "Number") = ![Number](Type-Number.png "Number"):teamPlayers()

Returns the number of players of the team associated with the team number (10 ops)

### ![Number](Type-Number.png "Number") = ![Number](Type-Number.png "Number"):teamDeaths()

Returns the number of deaths of the team associated with the team number (10 ops)

### ![Number](Type-Number.png "Number") = ![Number](Type-Number.png "Number"):teamFrags()

Returns the number of kills of the team associated with the team number (10 ops)

### setColor(![Number](Type-Number.png "Number") R, ![Number](Type-Number.png "Number") G, ![Number](Type-Number.png "Number") B)

Sets the color of the E2 chip (10 ops)

### applyForce(![Vector](Type-Vector.png "Vector") Force)

Applies force to the E2 chip according to the given vector's direction and magnitude (30 ops)

### applyOffsetForce(![Vector](Type-Vector.png "Vector") Force, ![Vector](Type-Vector.png "Vector") Position)

Applies force to the E2 chip according to the first vector from the location of the second (30 ops)

### applyAngForce(![Angle](Type-Angle.png "Angle") Angforce)

Applies torque to the E2 chip according to the given angle (30 ops)

### applyTorque(![Vector](Type-Vector.png "Vector") Torque)

Applies torque to the E2 chip according to the given vector, representing the torque axis, magnitude and direction (30 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):height()

Gets the height of a player or npc (10 ops)