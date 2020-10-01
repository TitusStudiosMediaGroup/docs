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

# Custom/prop

### ![Entity](Type-Entity.png "Entity") = propSpawn(![String](Type-String.png "String") Model, ![Number](Type-Number.png "Number") Frozen)

Use the model string or a template entity to spawn a prop. You can set the position and/or the rotation as well. The last number indicates frozen/unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![Entity](Type-Entity.png "Entity") Template, ![Number](Type-Number.png "Number") Frozen)

Entity template, Frozen Spawns a prop with the model of the template entity. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![String](Type-String.png "String") Model, ![Vector](Type-Vector.png "Vector") Pos, ![Number](Type-Number.png "Number") Frozen)

Model path, Position, Frozen Spawns a prop with the model denoted by the string filepath at the position denoted by the vector. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![Entity](Type-Entity.png "Entity") Template, ![Vector](Type-Vector.png "Vector") Pos, ![Number](Type-Number.png "Number") Frozen)

Entity template, Position, Frozen Spawns a prop with the model of the template entity at the position denoted by the vector. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![String](Type-String.png "String") Model, ![Angle](Type-Angle.png "Angle") Rot, ![Number](Type-Number.png "Number") Frozen)

Model path, Rotation, Frozen Spawns a prop with the model denoted by the string filepath and rotated to the angle given. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![Entity](Type-Entity.png "Entity") Template, ![Angle](Type-Angle.png "Angle") Rot, ![Number](Type-Number.png "Number") Frozen)

Rotation, Frozen Spawns a prop with the model of the template entity and rotated to the angle given. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![String](Type-String.png "String") Model, ![Vector](Type-Vector.png "Vector") Pos, ![Angle](Type-Angle.png "Angle") Rot, ![Number](Type-Number.png "Number") Frozen)

Model path, Position, Rotation, Frozen Spawns a prop with the model denoted by the string file path, at the position denoted by the vector, and rotated to the angle given. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = propSpawn(![Entity](Type-Entity.png "Entity") Template, ![Vector](Type-Vector.png "Vector") Pos, ![Angle](Type-Angle.png "Angle") Rot, ![Number](Type-Number.png "Number") Frozen)

Position, Rotation, Frozen Spawns a prop with the model of the template entity, at the position denoted by the vector, and rotated to the angle given. If frozen is 0, then it will spawn unfrozen. (40 ops)

### ![Entity](Type-Entity.png "Entity") = seatSpawn(![String](Type-String.png "String") Model, ![Number](Type-Number.png "Number") Frozen)

Model path, Frozen Spawns a prop with the model denoted by the string filepath. If frozen is 0, then it will spawn unfrozen. (60 ops)

### ![Entity](Type-Entity.png "Entity") = seatSpawn(![String](Type-String.png "String") Model, ![Vector](Type-Vector.png "Vector") Pos, ![Angle](Type-Angle.png "Angle") Rot, ![Number](Type-Number.png "Number") Frozen)

Model path, Frozen Spawns a prop with the model denoted by the string filepath. If frozen is 0, then it will spawn unfrozen. (60 ops)

### ![Entity](Type-Entity.png "Entity"):propDelete()

Deletes the specified prop. (10 ops)

### ![Entity](Type-Entity.png "Entity"):propBreak()

Breaks/Explodes breakable/explodable props (Useful for Mines). (10 ops)

### ![Entity](Type-Entity.png "Entity"):use()

Simulates a player pressing their use key on the entity. (10 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):propDelete()

Deletes all the props in the given table, returns the amount of props deleted. (30 ops)

### ![Number](Type-Number.png "Number") = ![Array](Type-Array.png "Array"):propDelete()

Deletes all the props in the given array, returns the amount of props deleted. (30 ops)

### propDeleteAll()

Removes all entities spawned by this E2 (30 ops)

### ![Entity](Type-Entity.png "Entity"):propManipulate(![Vector](Type-Vector.png "Vector") Pos, ![Angle](Type-Angle.png "Angle") Rot, ![Number](Type-Number.png "Number") Freeze, ![Number](Type-Number.png "Number") Gravity, ![Number](Type-Number.png "Number") Notsolid)

Allows to do any single prop core function in one term (position, rotation, freeze, gravity, notsolid) (10 ops)

### ![Entity](Type-Entity.png "Entity"):propFreeze(![Number](Type-Number.png "Number") Freeze)

Passing 0 unfreezes the entity, everything else freezes it. (10 ops)

### ![Entity](Type-Entity.png "Entity"):propNotSolid(![Number](Type-Number.png "Number") Notsolid)

Passing 0 makes the entity solid, everything else makes it non-solid. (10 ops)

### ![Entity](Type-Entity.png "Entity"):propDraw(![Number](Type-Number.png "Number") Drawenable)

Passing 0 disables rendering for the entity (makes it really invisible) (10 ops)

### ![Entity](Type-Entity.png "Entity"):propShadow(![Number](Type-Number.png "Number") Shadowenable)

Passing 0 disables rendering for the entity's shadow (10 ops)

### ![Entity](Type-Entity.png "Entity"):propGravity(![Number](Type-Number.png "Number") Gravity)

Passing 0 makes the entity weightless, everything else makes it weighty. (10 ops)

### ![Entity](Type-Entity.png "Entity"):propDrag(![Number](Type-Number.png "Number") Drag)

Passing 0 makes the entity not be affected by drag (10 ops)

### ![Entity](Type-Entity.png "Entity"):propInertia(![Vector](Type-Vector.png "Vector") Inertia)

Sets the directional inertia (10 ops)

### ![Entity](Type-Entity.png "Entity"):propSetBuoyancy(![Number](Type-Number.png "Number") Buoyancy)

Sets the prop's buoyancy ratio from 0 to 1 (10 ops)

### ![Entity](Type-Entity.png "Entity"):propSetFriction(![Number](Type-Number.png "Number") Friction)

Sets prop's friction coefficient (default is 1) (10 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):propGetFriction()

Gets prop's friction coefficient (10 ops)

### ![Entity](Type-Entity.png "Entity"):propSetElasticity(![Number](Type-Number.png "Number") Elasticity)

Sets prop's elasticity coefficient (default is 1) (10 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):propGetElasticity()

Gets prop's elasticity coefficient (10 ops)

### ![Entity](Type-Entity.png "Entity"):propMakePersistent(![Number](Type-Number.png "Number") Persistent)

Setting to 1 will make the prop persistent. (10 ops)

### ![Entity](Type-Entity.png "Entity"):propPhysicalMaterial(![String](Type-String.png "String") Physprop)

Changes the surface material of a prop (eg. wood, metal, ... See Material_surface_properties ). (10 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):propPhysicalMaterial()

Returns the surface material of a prop. (10 ops)

### ![Entity](Type-Entity.png "Entity"):propSetVelocity(![Vector](Type-Vector.png "Vector") Velocity)

Sets the velocity of the prop for the next iteration (10 ops)

### ![Entity](Type-Entity.png "Entity"):propSetVelocityInstant(![Vector](Type-Vector.png "Vector") Velocity)

Sets the initial velocity of the prop (10 ops)

### ![Entity](Type-Entity.png "Entity"):propStatic(![Number](Type-Number.png "Number") Static)

Sets to 1 to make the entity static (disables movement, physgun, unfreeze, drive...) or 0 to cancel. (10 ops)

### ![Entity](Type-Entity.png "Entity"):reposition(![Vector](Type-Vector.png "Vector") Pos)

Deprecated. Kept for backwards-compatibility. (20 ops)

### ![Entity](Type-Entity.png "Entity"):setPos(![Vector](Type-Vector.png "Vector") Pos)

Sets the position of an entity. (20 ops)

### ![Entity](Type-Entity.png "Entity"):rerotate(![Angle](Type-Angle.png "Angle") Rot)

Deprecated. Kept for backwards-compatibility. (20 ops)

### ![Entity](Type-Entity.png "Entity"):setAng(![Angle](Type-Angle.png "Angle") Rot)

Set the rotation of an entity. (20 ops)

### ![Entity](Type-Entity.png "Entity"):parentTo(![Entity](Type-Entity.png "Entity") Target)

Parents one entity to another. (20 ops)

### ![Entity](Type-Entity.png "Entity"):deparent()

Unparents an entity, so it moves freely again. (5 ops)

### ![Entity](Type-Entity.png "Entity"):parentTo()

Parents one entity to another. (5 ops)

### propSpawnEffect(![Number](Type-Number.png "Number") On)

Set to 1 to enable prop spawn effect, 0 to disable. (1 ops)

### propSpawnUndo(![Number](Type-Number.png "Number") On)

Set to 0 to force prop removal on E2 shutdown, and suppress Undo entries for props. (1 ops)

### ![Number](Type-Number.png "Number") = propCanCreate()

Returns 1 when propSpawn() will successfully spawn a prop until the limit is reached. (1 ops)