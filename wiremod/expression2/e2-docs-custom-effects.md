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

# Custom/effects

### Effect = effect()

Creates and returns new effect (1 ops)

### Effect = Effect:setOrigin(![Vector](Type-Vector.png "Vector") Pos)

Sets the origin of the effect (1 ops)

### Effect = Effect:setStart(![Vector](Type-Vector.png "Vector") Pos)

Sets the start of the effect (1 ops)

### Effect = Effect:setMagnitude(![Number](Type-Number.png "Number") Mag)

Sets the magnitude of the effect (1 ops)

### Effect = Effect:setAngles(![Angle](Type-Angle.png "Angle") Ang)

Sets the angle of the effect (1 ops)

### Effect = Effect:setScale(![Number](Type-Number.png "Number") Scale)

Sets the scale of the effect (1 ops)

### Effect = Effect:setEntity(![Entity](Type-Entity.png "Entity") Ent)

Sets the entity of the effect (1 ops)

### Effect = Effect:setNormal(![Vector](Type-Vector.png "Vector") Norm)

Sets the normalized direction vector of the effect (1 ops)

### Effect = Effect:setSurfaceProp(![Number](Type-Number.png "Number") Prop)

Sets the surface property index of the effect (1 ops)

### Effect = Effect:setRadius(![Number](Type-Number.png "Number") Radius)

Sets the radius of the effect (1 ops)

### Effect = Effect:setMaterialIndex(![Number](Type-Number.png "Number") Index)

Sets the material index of the effect (1 ops)

### Effect = Effect:setHitBox(![Number](Type-Number.png "Number") Index)

Sets the hit box index of the effect (1 ops)

### Effect = Effect:setFlags(![Number](Type-Number.png "Number") Flags)

Sets the flags of the effect (1 ops)

### Effect = Effect:setEntIndex(![Number](Type-Number.png "Number") Index)

Sets the entity of the effect via its index (1 ops)

### Effect = Effect:setDamageType(![Number](Type-Number.png "Number") Index)

Sets the damage type of the effect. See DMG_ Enums on GMod Wiki (1 ops)

### Effect = Effect:setColor(![Number](Type-Number.png "Number") Index)

Sets the color of the effect. Color is represented by a byte (1 ops)

### Effect = Effect:setAttachment(![Number](Type-Number.png "Number") Index)

Creates new attachment ID for the effect (1 ops)

### Effect:play(![String](Type-String.png "String") Name)

Plays the effect with given name (eg. watersplash) (1 ops)