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

# Globalvars

### Gtable = gTable(![String](Type-String.png "String") Groupname)

Returns the gTable. The string determines group (1 ops)

### Gtable = gTable(![String](Type-String.png "String") Groupname, ![Number](Type-Number.png "Number") Shared)

Returns the gTable. The string determines group, and the number determines wether or not the table should be shared (1 ops)

### Gtable = gTableSafe(![Number](Type-Number.png "Number") Shared)

Returns a safe gTable which group is a numerical hash created from the code of the E2 itself (1 ops)

### gRemoveAll()

Removes all non-shared variables and group tables you have created (5 ops)

### Gtable:clear()

Clears the gTable (5 ops)

### ![Number](Type-Number.png "Number") = Gtable:count()

Returns the number of entries in the gTable. Does not add the entries in subtables (5 ops)

### ![Table](Type-Table.png "Table") = Gtable:toTable()

Converts the GTable into a table (5 ops)

### ![Bone](Type-Bone.png "Bone") = Gtable:removeBone(![String](Type-String.png "String"))

Removes and returns the variable of the bone type at the index S (5 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = Gtable:removeMatrix4(![String](Type-String.png "String"))

Removes and returns the variable of the matrix4 type at the index S (5 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = Gtable:removeQuaternion(![String](Type-String.png "String"))

Removes and returns the variable of the quaternion type at the index S (5 ops)

### ![Entity](Type-Entity.png "Entity") = Gtable:removeEntity(![String](Type-String.png "String"))

Removes and returns the variable of the entity type at the index S (5 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = Gtable:removeMatrix2(![String](Type-String.png "String"))

Removes and returns the variable of the matrix2 type at the index S (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = Gtable:removeVector4(![String](Type-String.png "String"))

Removes and returns the variable of the vector4 type at the index S (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = Gtable:removeComplex(![String](Type-String.png "String"))

Removes and returns the variable of the complex type at the index S (5 ops)

### ![Matrix](Type-Matrix.png "Matrix") = Gtable:removeMatrix(![String](Type-String.png "String"))

Removes and returns the variable of the matrix type at the index S (5 ops)

### ![WireLink](Type-WireLink.png "WireLink") = Gtable:removeWirelink(![String](Type-String.png "String"))

Removes and returns the variable of the wirelink type at the index S (5 ops)

### Tracedata = Gtable:removeTracedata(![String](Type-String.png "String"))

Removes and returns the variable of the tracedata type at the index S (5 ops)

### ![Vector](Type-Vector.png "Vector") = Gtable:removeVector(![String](Type-String.png "String"))

Removes and returns the variable of the vector type at the index S (5 ops)

### ![Angle](Type-Angle.png "Angle") = Gtable:removeAngle(![String](Type-String.png "String"))

Removes and returns the variable of the angle type at the index S (5 ops)

### Ftrace = Gtable:removeFtrace(![String](Type-String.png "String"))

Removes and returns the variable of the ftrace type at the index S (5 ops)

### Stcontrol = Gtable:removeStcontrol(![String](Type-String.png "String"))

Removes and returns the variable of the stcontrol type at the index S (5 ops)

### ![String](Type-String.png "String") = Gtable:removeString(![String](Type-String.png "String"))

Removes and returns the variable of the string type at the index S (5 ops)

### ![RangerData](Type-RangerData.png "RangerData") = Gtable:removeRanger(![String](Type-String.png "String"))

Removes and returns the variable of the ranger type at the index S (5 ops)

### Effect = Gtable:removeEffect(![String](Type-String.png "String"))

Removes and returns the variable of the effect type at the index S (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = Gtable:removeVector2(![String](Type-String.png "String"))

Removes and returns the variable of the vector2 type at the index S (5 ops)

### ![Array](Type-Array.png "Array") = Gtable:removeArray(![String](Type-String.png "String"))

Removes and returns the variable of the array type at the index S (5 ops)

### ![Number](Type-Number.png "Number") = Gtable:removeNumber(![String](Type-String.png "String"))

Removes and returns the variable of the number type at the index S (5 ops)

### ![Table](Type-Table.png "Table") = Gtable:removeTable(![String](Type-String.png "String"))

Removes and returns the variable of the table type at the index S (5 ops)

### gRemoveAllWirelinks()

Removes all variables of the wirelink type in your non-shared table (5 ops)

### gRemoveAllMatrixs()

Removes all variables of the matrix type in your non-shared table (5 ops)

### gRemoveAllTables()

Removes all variables of the table type in your non-shared table (5 ops)

### gRemoveAllTracedatas()

Removes all variables of the tracedata type in your non-shared table (5 ops)

### gRemoveAllVector2s()

Removes all variables of the vector2 type in your non-shared table (5 ops)

### gRemoveAllNumbers()

Removes all variables of the number type in your non-shared table (5 ops)

### gRemoveAllQuaternions()

Removes all variables of the quaternion type in your non-shared table (5 ops)

### gRemoveAllMatrix2s()

Removes all variables of the matrix2 type in your non-shared table (5 ops)

### gRemoveAllBones()

Removes all variables of the bone type in your non-shared table (5 ops)

### gRemoveAllArrays()

Removes all variables of the array type in your non-shared table (5 ops)

### gRemoveAllStcontrols()

Removes all variables of the stcontrol type in your non-shared table (5 ops)

### gRemoveAllVectors()

Removes all variables of the vector type in your non-shared table (5 ops)

### gRemoveAllStrings()

Removes all variables of the string type in your non-shared table (5 ops)

### gRemoveAllEffects()

Removes all variables of the effect type in your non-shared table (5 ops)

### gRemoveAllComplexs()

Removes all variables of the complex type in your non-shared table (5 ops)

### gRemoveAllMatrix4s()

Removes all variables of the matrix4 type in your non-shared table (5 ops)

### gRemoveAllFtraces()

Removes all variables of the ftrace type in your non-shared table (5 ops)

### gRemoveAllEntitys()

Removes all variables of the entity type in your non-shared table (5 ops)

### gRemoveAllVector4s()

Removes all variables of the vector4 type in your non-shared table (5 ops)

### gRemoveAllRangers()

Removes all variables of the ranger type in your non-shared table (5 ops)

### gRemoveAllAngles()

Removes all variables of the angle type in your non-shared table (5 ops)

### gRemoveAllFtraces(![String](Type-String.png "String"))

Removes all variables of the ftrace type in your non-shared table in group S (5 ops)

### gRemoveAllNumbers(![String](Type-String.png "String"))

Removes all variables of the number type in your non-shared table in group S (5 ops)

### gRemoveAllMatrix4s(![String](Type-String.png "String"))

Removes all variables of the matrix4 type in your non-shared table in group S (5 ops)

### gRemoveAllWirelinks(![String](Type-String.png "String"))

Removes all variables of the wirelink type in your non-shared table in group S (5 ops)

### gRemoveAllMatrix2s(![String](Type-String.png "String"))

Removes all variables of the matrix2 type in your non-shared table in group S (5 ops)

### gRemoveAllVector4s(![String](Type-String.png "String"))

Removes all variables of the vector4 type in your non-shared table in group S (5 ops)

### gRemoveAllEntitys(![String](Type-String.png "String"))

Removes all variables of the entity type in your non-shared table in group S (5 ops)

### gRemoveAllAngles(![String](Type-String.png "String"))

Removes all variables of the angle type in your non-shared table in group S (5 ops)

### gRemoveAllArrays(![String](Type-String.png "String"))

Removes all variables of the array type in your non-shared table in group S (5 ops)

### gRemoveAllStcontrols(![String](Type-String.png "String"))

Removes all variables of the stcontrol type in your non-shared table in group S (5 ops)

### gRemoveAllVector2s(![String](Type-String.png "String"))

Removes all variables of the vector2 type in your non-shared table in group S (5 ops)

### gRemoveAllComplexs(![String](Type-String.png "String"))

Removes all variables of the complex type in your non-shared table in group S (5 ops)

### gRemoveAllTracedatas(![String](Type-String.png "String"))

Removes all variables of the tracedata type in your non-shared table in group S (5 ops)

### gRemoveAllBones(![String](Type-String.png "String"))

Removes all variables of the bone type in your non-shared table in group S (5 ops)

### gRemoveAllRangers(![String](Type-String.png "String"))

Removes all variables of the ranger type in your non-shared table in group S (5 ops)

### gRemoveAllMatrixs(![String](Type-String.png "String"))

Removes all variables of the matrix type in your non-shared table in group S (5 ops)

### gRemoveAllEffects(![String](Type-String.png "String"))

Removes all variables of the effect type in your non-shared table in group S (5 ops)

### gRemoveAllQuaternions(![String](Type-String.png "String"))

Removes all variables of the quaternion type in your non-shared table in group S (5 ops)

### gRemoveAllStrings(![String](Type-String.png "String"))

Removes all variables of the string type in your non-shared table in group S (5 ops)

### gRemoveAllTables(![String](Type-String.png "String"))

Removes all variables of the table type in your non-shared table in group S (5 ops)

### gRemoveAllVectors(![String](Type-String.png "String"))

Removes all variables of the vector type in your non-shared table in group S (5 ops)

### gSetGroup(![String](Type-String.png "String") Groupname)

Sets the E2's current group. Does persist (1 ops)

### ![String](Type-String.png "String") = gGetGroup()

Gets the E2's current group (1 ops)

### gShare(![Number](Type-Number.png "Number") Share)

Sets wether or not you want to share the variables. (1/0) Remember that there are two tables for each group: one which is shared and one which is not; values do not transition between the two (1 ops)

### ![Number](Type-Number.png "Number") = gGetShare()

Returns 1/0 (1 ops)

### gResetGroup()

Resets the group back to "default" (1 ops)

### gSetNum(![String](Type-String.png "String"), ![Number](Type-Number.png "Number"))

Sets a variable of the number type at index S in the current group (8 ops)

### gSetStr(![String](Type-String.png "String"), ![String](Type-String.png "String"))

Sets a variable of the string type at index S in the current group (8 ops)

### gSetAng(![String](Type-String.png "String"), ![Angle](Type-Angle.png "Angle"))

Sets a variable of the angle type at index S in the current group (8 ops)

### gSetEnt(![String](Type-String.png "String"), ![Entity](Type-Entity.png "Entity"))

Sets a variable of the entity type at index S in the current group (8 ops)

### gSetVec(![String](Type-String.png "String"), ![Vector](Type-Vector.png "Vector"))

Sets a variable of the vector type at index S in the current group (8 ops)

### ![String](Type-String.png "String") = gGetStr(![String](Type-String.png "String"))

Gets a variable of the string type from index S in the current group (8 ops)

### ![Angle](Type-Angle.png "Angle") = gGetAng(![String](Type-String.png "String"))

Gets a variable of the angle type from index S in the current group (8 ops)

### ![Vector](Type-Vector.png "Vector") = gGetVec(![String](Type-String.png "String"))

Gets a variable of the vector type from index S in the current group (8 ops)

### ![Entity](Type-Entity.png "Entity") = gGetEnt(![String](Type-String.png "String"))

Gets a variable of the entity type from index S in the current group (8 ops)

### ![Number](Type-Number.png "Number") = gGetNum(![String](Type-String.png "String"))

Gets a variable of the number type from index S in the current group (8 ops)

### gSetVec(![Number](Type-Number.png "Number"), ![Vector](Type-Vector.png "Vector"))

Exactly the same as gSetVec(N:toString(),vector) (8 ops)

### gSetEnt(![Number](Type-Number.png "Number"), ![Entity](Type-Entity.png "Entity"))

Exactly the same as gSetEnt(N:toString(),entity) (8 ops)

### gSetNum(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Exactly the same as gSetNum(N:toString(),number) (8 ops)

### gSetStr(![Number](Type-Number.png "Number"), ![String](Type-String.png "String"))

Exactly the same as gSetStr(N:toString(),string) (8 ops)

### gSetAng(![Number](Type-Number.png "Number"), ![Angle](Type-Angle.png "Angle"))

Exactly the same as gSetAng(N:toString(),angle) (8 ops)

### ![Entity](Type-Entity.png "Entity") = gGetEnt(![Number](Type-Number.png "Number"))

Exactly the same as gGetEnt(N:toString()) (8 ops)

### ![Number](Type-Number.png "Number") = gGetNum(![Number](Type-Number.png "Number"))

Exactly the same as gGetNum(N:toString()) (8 ops)

### ![Angle](Type-Angle.png "Angle") = gGetAng(![Number](Type-Number.png "Number"))

Exactly the same as gGetAng(N:toString()) (8 ops)

### ![Vector](Type-Vector.png "Vector") = gGetVec(![Number](Type-Number.png "Number"))

Exactly the same as gGetVec(N:toString()) (8 ops)

### ![String](Type-String.png "String") = gGetStr(![Number](Type-Number.png "Number"))

Exactly the same as gGetStr(N:toString()) (8 ops)

### ![Entity](Type-Entity.png "Entity") = gDeleteEnt(![String](Type-String.png "String"))

Removes and returns the variable of the entity type at the index S in the current group (8 ops)

### ![String](Type-String.png "String") = gDeleteStr(![String](Type-String.png "String"))

Removes and returns the variable of the string type at the index S in the current group (8 ops)

### ![Angle](Type-Angle.png "Angle") = gDeleteAng(![String](Type-String.png "String"))

Removes and returns the variable of the angle type at the index S in the current group (8 ops)

### ![Number](Type-Number.png "Number") = gDeleteNum(![String](Type-String.png "String"))

Removes and returns the variable of the number type at the index S in the current group (8 ops)

### ![Vector](Type-Vector.png "Vector") = gDeleteVec(![String](Type-String.png "String"))

Removes and returns the variable of the vector type at the index S in the current group (8 ops)

### ![Vector](Type-Vector.png "Vector") = gDeleteVec(![Number](Type-Number.png "Number"))

Exactly the same as gDeleteVec(N:toString()) (8 ops)

### ![Angle](Type-Angle.png "Angle") = gDeleteAng(![Number](Type-Number.png "Number"))

Exactly the same as gDeleteAng(N:toString()) (8 ops)

### ![Number](Type-Number.png "Number") = gDeleteNum(![Number](Type-Number.png "Number"))

Exactly the same as gDeleteNum(N:toString()) (8 ops)

### ![String](Type-String.png "String") = gDeleteStr(![Number](Type-Number.png "Number"))

Exactly the same as gDeleteStr(N:toString()) (8 ops)

### ![Entity](Type-Entity.png "Entity") = gDeleteEnt(![Number](Type-Number.png "Number"))

Exactly the same as gDeleteEnt(N:toString()) (8 ops)

### gDeleteAllAng()

Exactly the same as gRemoveAllAngles(S) (Except it removes in the group set by gSetGroup instead of using the group as an argument) (5 ops)

### gDeleteAllEnt()

Exactly the same as gRemoveAllEntitys(S) (Except it removes in the group set by gSetGroup instead of using the group as an argument) (5 ops)

### gDeleteAllNum()

Exactly the same as gRemoveAllNumbers(S) (Except it removes in the group set by gSetGroup instead of using the group as an argument) (5 ops)

### gDeleteAllVec()

Exactly the same as gRemoveAllVectors(S) (Except it removes in the group set by gSetGroup instead of using the group as an argument) (5 ops)

### gDeleteAllStr()

Exactly the same as gRemoveAllStrings(S) (Except it removes in the group set by gSetGroup instead of using the group as an argument) (5 ops)