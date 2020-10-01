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

# Custom/constraintcore

### enableConstraintUndo(![Number](Type-Number.png "Number") State)

 (1 ops)

### axis(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2)

Creates an axis constraint between two entities at vectors local to each entity (30 ops)

### axis(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Friction)

Creates an axis constraint between two entities at vectors local to each entity with friction (30 ops)

### axis(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Friction, ![Vector](Type-Vector.png "Vector") Localaxis)

Creates an axis constraint between two entities at vectors local to each entity with friction and local rotation axis (30 ops)

### ballsocket(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V, ![Entity](Type-Entity.png "Entity") Ent2)

 (30 ops)

### ballsocket(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V, ![Entity](Type-Entity.png "Entity") Ent2, ![Number](Type-Number.png "Number") Friction)

 (30 ops)

### ballsocket(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") Mins, ![Vector](Type-Vector.png "Vector") Maxs, ![Vector](Type-Vector.png "Vector") Frictions)

Creates an AdvBallsocket constraint between two entities at a vector local to ent1, using the specified mins, maxs, and frictions (30 ops)

### ballsocket(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") Mins, ![Vector](Type-Vector.png "Vector") Maxs, ![Vector](Type-Vector.png "Vector") Frictions, ![Number](Type-Number.png "Number") Rotateonly)

Creates an AdvBallsocket constraint between two entities at a vector local to ent1, using the specified mins, maxs, frictions, rotateonly (30 ops)

### weldAng(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V, ![Entity](Type-Entity.png "Entity") Ent2)

 (30 ops)

### winch(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Width)

 (30 ops)

### hydraulic(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Width)

Creates a hydraulic constraint with a referenceid, between two entities, at vectors local to each (30 ops)

### hydraulic(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Constant, ![Number](Type-Number.png "Number") Damping, ![String](Type-String.png "String") Mat, ![Number](Type-Number.png "Number") Width, ![Number](Type-Number.png "Number") Stretch)

Creates a hydraulic constraint with a referenceid, between two entities, at vectors local to each, with constant, damping, and stretch only (30 ops)

### hydraulic(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Constant, ![Number](Type-Number.png "Number") Damping, ![Number](Type-Number.png "Number") Rdamping, ![String](Type-String.png "String") Mat, ![Number](Type-Number.png "Number") Width, ![Number](Type-Number.png "Number") Stretch)

Creates a hydraulic constraint with a referenceid, between two entities, at vectors local to each, with constant, damping, relative damping and stretch only (30 ops)

### rope(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2)

Creates a rope constraint with a referenceid, between two entities, at vectors local to each (30 ops)

### rope(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Addlength, ![Number](Type-Number.png "Number") Width, ![String](Type-String.png "String") Mat)

Creates a rope constraint with a referenceid, between two entities, at vectors local to each with add length, width, and material (30 ops)

### rope(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Addlength, ![Number](Type-Number.png "Number") Width, ![String](Type-String.png "String") Mat, ![Number](Type-Number.png "Number") Rigid)

Creates a rope constraint with a referenceid, between two entities, at vectors local to each with add length, width, material, and rigidity (30 ops)

### ![Entity](Type-Entity.png "Entity"):setLength(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Length)

Sets the length of a winch/hydraulic/rope stored in this entity at a referenceid (5 ops)

### ![Entity](Type-Entity.png "Entity"):setConstant(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Constant)

 (5 ops)

### ![Entity](Type-Entity.png "Entity"):setConstant(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Constant, ![Number](Type-Number.png "Number") Damping)

 (5 ops)

### ![Entity](Type-Entity.png "Entity"):setDamping(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Damping)

 (5 ops)

### slider(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2)

 (30 ops)

### slider(![Entity](Type-Entity.png "Entity") Ent1, ![Vector](Type-Vector.png "Vector") V1, ![Entity](Type-Entity.png "Entity") Ent2, ![Vector](Type-Vector.png "Vector") V2, ![Number](Type-Number.png "Number") Width)

 (30 ops)

### noCollide(![Entity](Type-Entity.png "Entity") Ent1, ![Entity](Type-Entity.png "Entity") Ent2)

 (30 ops)

### noCollideAll(![Entity](Type-Entity.png "Entity") Ent, ![Number](Type-Number.png "Number") State)

 (30 ops)

### weld(![Entity](Type-Entity.png "Entity") Ent1, ![Entity](Type-Entity.png "Entity") Ent2)

 (30 ops)

### ![Entity](Type-Entity.png "Entity"):constraintBreak()

Breaks all constraints of all types on an entity (5 ops)

### ![Entity](Type-Entity.png "Entity"):constraintBreak(![Entity](Type-Entity.png "Entity") Ent2)

Breaks all constraints between two entities (5 ops)

### ![Entity](Type-Entity.png "Entity"):constraintBreak(![String](Type-String.png "String") Type)

Breaks all constraints of a type (weld, axis, nocollide, ballsocket) on an entity (5 ops)

### ![Entity](Type-Entity.png "Entity"):constraintBreak(![String](Type-String.png "String") Type, ![Entity](Type-Entity.png "Entity") Ent2)

Breaks a constraint of a type (weld, axis, nocollide, ballsocket) between two entities (5 ops)