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

# Constraint

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):getConstraints()

Returns an array with all entities directly or indirectly constrained to E, except E itself. Deprecated, use E:getConnectedEntities(...) instead. (20 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):getConnectedEntities(... This)

Returns an array with all entities directly or indirectly constrained or parented to E, including E itself. (20 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):getConnectedEntities(![Array](Type-Array.png "Array") Filters)

Returns an array with all entities directly or indirectly constrained or parented to E, including E itself. (20 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):hasConstraints()

Returns the number of the constraints E has (5 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):hasConstraints(![String](Type-String.png "String") Constrainttype)

Returns the number of the constraints E has with the given constraint type (5 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):isConstrained()

Returns 1 if E has constraints, 0 if not (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):isWeldedTo()

Returns the first entity E was welded to (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):isWeldedTo(![Number](Type-Number.png "Number") Index)

Returns the Nth entity E was welded to (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):isConstrainedTo()

Returns the first entity E was constrained to (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):isConstrainedTo(![Number](Type-Number.png "Number") Index)

Returns the Nth entity E was constrained to (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):isConstrainedTo(![String](Type-String.png "String") Constrainttype)

Returns the first entity E was constrained to with the given constraint type (see the types list below) (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):isConstrainedTo(![String](Type-String.png "String") Constrainttype, ![Number](Type-Number.png "Number") Index)

Returns the Nth entity E was constrained to with the given constraint type (see the types list below) (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):parent()

Returns the entity E is parented to (5 ops)

### ![Bone](Type-Bone.png "Bone") = ![Entity](Type-Entity.png "Entity"):parentBone()

Returns the bone E is parented to (5 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):children()

Returns an array containing all the children of the entity - that is, every entity whose parent is this entity (20 ops)