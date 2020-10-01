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

# Weapon

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):weapon()

Returns the weapon that player E is currently holding (2 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):weapon(![String](Type-String.png "String") Weaponclassname)

Returns the weapon with specified class of player E (2 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):weapons()

Returns the weapons that player E has (2 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):primaryAmmoType()

Returns the name of the primary weapon's ammo (2 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):secondaryAmmoType()

Returns the name of the secondary weapon's ammo (2 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):ammoCount(![String](Type-String.png "String") Ammo_type)

Returns the amount of stored ammo of type S on player E, excluding current clip (2 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):clip1()

Returns the amount of ammo in the primary clip of weapon E, -1 if there is no primary clip (2 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):clip2()

Returns the amount of ammo in the secondary clip of weapon E, -1 if there is no secondary clip 1) (2 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):tool()

returns the name of the tool the player E is currently holding (2 ops)