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

# Table

### ![Table](Type-Table.png "Table") = table(...)

 (1 ops)

### ![Table](Type-Table.png "Table"):clear()

Clears the table (1 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):count()

Returns the number of entries in the table. Does not add the entries in subtables (1 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):ncount()

Returns the number of sequential numerical indexes (3 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):exists(![Number](Type-Number.png "Number") Index)

Returns 1 if the table contains any value at specified index (1 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):exists(![String](Type-String.png "String") Index)

Returns 1 if the table contains any value at specified index (1 ops)

### printTable(![Table](Type-Table.png "Table") Tbl)

Prints a table like the lua function PrintTable does, except to the chat area (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):flip()

Returns a flipped copy of the table. Only affects string values in the array part and number values in the table part (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):typeids()

Returns a new table with the typeids of the table (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):remove(![Number](Type-Number.png "Number") Index)

Removes the specified entry from the array-part and returns 1 if removed (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):remove(![String](Type-String.png "String") Index)

Removes the specified entry from the table-part and returns 1 if removed (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):unset(![String](Type-String.png "String") Index)

Force removes the specified entry from the table-part, without moving subsequent entries down and returns 1 if removed (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):unset(![Number](Type-Number.png "Number") Index)

Force removes the specified entry from the array-part, without moving subsequent entries down and returns 1 if removed (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):clipToTypeid(![String](Type-String.png "String") Typeid)

Removes all entries not of the specified type (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):clipFromTypeid(![String](Type-String.png "String") Typeid)

Removes all entries of the specified type (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):clone()

Returns a copy of the table (10 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):id()

Returns the unique ID of the table (1 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):toString()

Formats the table as a human-readable string (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):add(![Table](Type-Table.png "Table") Rv2)

Adds the contents of the second table to the end of the first table. Returns new table (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):merge(![Table](Type-Table.png "Table") Rv2)

Merges T2 with T. Any variables with the same indexes are overwritten by T2's variables (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):difference(![Table](Type-Table.png "Table") Rv2)

Removes all variables with keys that exist in T2 (5 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):intersect(![Table](Type-Table.png "Table") Rv2)

Removes all variables with keys which don't exist in T2 (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):pop()

Removes the last entry in the array-part and returns 1 if removed (3 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):shift()

Removes the first element of the table; all other entries will move down one address and returns 1 if removed (3 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):min()

Returns the smallest numerical entry in the array-part (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):max()

Returns the largest numerical entry in the array-part (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):maxIndex()

Returns the index of the largest numerical entry in the array-part (5 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):minIndex()

Returns the index of the smallest numerical entry in the array-part (5 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):typeidsArray()

Returns an array with the typeids of the array-part of the table (5 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):toArray()

Converts the table into an array. (Note that there is no R:totable() function because E2 arrays do not save typeids) (5 ops)

### ![Table](Type-Table.png "Table") = findToTable()

Inserts the finds from an entity discovery event into an table's array-part and returns it. (Basically the same as findToArray()) (20 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):concat()

Concatenates the array-part of the table (1 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):concat(![String](Type-String.png "String") Delimiter)

Concatenates the array-part of the table, with a string delimiter (1 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):concat(![String](Type-String.png "String") Delimiter, ![Number](Type-Number.png "Number") Startindex)

Concatenates the array-part of the table, starting at index N, with string S in between each (1 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):concat(![String](Type-String.png "String") Delimiter, ![Number](Type-Number.png "Number") Startindex, ![Number](Type-Number.png "Number") Endindex)

Concatenates the array-part of the table, starting at index N1 and ending at N2, with string S in between each (1 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):concat(![Number](Type-Number.png "Number") Startindex)

Concatenates the array-part of the table, starting at index N (1 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):concat(![Number](Type-Number.png "Number") Startindex, ![Number](Type-Number.png "Number") Endindex)

Concatenates the array-part of the table, starting at index N1 and ending at N2 (1 ops)

### ![Table](Type-Table.png "Table") = invert(![Array](Type-Array.png "Array") Arr)

Inverts the array, creating a lookup table (5 ops)

### ![Table](Type-Table.png "Table") = invert(![Table](Type-Table.png "Table") Tbl)

Inverts the table, creating a lookup table (5 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):keys()

Returns an array with the keys of the table (5 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):values()

Returns an array with the values of the table (tables and arrays, which arrays do not support, are discarded) (5 ops)

### Ftrace = ![Table](Type-Table.png "Table"):removeFtrace(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ![Table](Type-Table.png "Table"):removeMatrix(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ![Table](Type-Table.png "Table"):removeMatrix4(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### Effect = ![Table](Type-Table.png "Table"):removeEffect(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Bone](Type-Bone.png "Bone") = ![Table](Type-Table.png "Table"):removeBone(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):removeTable(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### Stcontrol = ![Table](Type-Table.png "Table"):removeStcontrol(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Table](Type-Table.png "Table"):removeVector2(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ![Table](Type-Table.png "Table"):removeQuaternion(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Angle](Type-Angle.png "Angle") = ![Table](Type-Table.png "Table"):removeAngle(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):removeString(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### Tracedata = ![Table](Type-Table.png "Table"):removeTracedata(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ![Table](Type-Table.png "Table"):removeComplex(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ![Table](Type-Table.png "Table"):removeMatrix2(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Table](Type-Table.png "Table"):removeVector4(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ![Table](Type-Table.png "Table"):removeWirelink(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):removeArray(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ![Table](Type-Table.png "Table"):removeRanger(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Entity](Type-Entity.png "Entity") = ![Table](Type-Table.png "Table"):removeEntity(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Vector](Type-Vector.png "Vector") = ![Table](Type-Table.png "Table"):removeVector(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):removeNumber(![String](Type-String.png "String"))

Removes the variable at the specified string index, with the specified type, and returns it (8 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):removeTable(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ![Table](Type-Table.png "Table"):removeQuaternion(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ![Table](Type-Table.png "Table"):removeRanger(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### Effect = ![Table](Type-Table.png "Table"):removeEffect(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ![Table](Type-Table.png "Table"):removeComplex(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ![Table](Type-Table.png "Table"):removeMatrix2(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Table](Type-Table.png "Table"):removeVector4(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### Tracedata = ![Table](Type-Table.png "Table"):removeTracedata(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):removeArray(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Table](Type-Table.png "Table"):removeVector2(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Bone](Type-Bone.png "Bone") = ![Table](Type-Table.png "Table"):removeBone(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### Stcontrol = ![Table](Type-Table.png "Table"):removeStcontrol(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Angle](Type-Angle.png "Angle") = ![Table](Type-Table.png "Table"):removeAngle(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ![Table](Type-Table.png "Table"):removeWirelink(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Vector](Type-Vector.png "Vector") = ![Table](Type-Table.png "Table"):removeVector(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Entity](Type-Entity.png "Entity") = ![Table](Type-Table.png "Table"):removeEntity(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):removeString(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ![Table](Type-Table.png "Table"):removeMatrix(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):removeNumber(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ![Table](Type-Table.png "Table"):removeMatrix4(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### Ftrace = ![Table](Type-Table.png "Table"):removeFtrace(![Number](Type-Number.png "Number"))

Removes the variable at the specified numerical index, with the specified type, and returns it. All sequential keys will be moved down to fill the gap (8 ops)

### ![Table](Type-Table.png "Table"):pushVector4(![Vector4](Type-Vector4.png "Vector4"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushVector2(![Vector2](Type-Vector2.png "Vector2"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushTracedata(Tracedata)

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushEffect(Effect)

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushTable(![Table](Type-Table.png "Table"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushArray(![Array](Type-Array.png "Array"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushComplex(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushNumber(![Number](Type-Number.png "Number"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushString(![String](Type-String.png "String"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushWirelink(![WireLink](Type-WireLink.png "WireLink"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushRanger(![RangerData](Type-RangerData.png "RangerData"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushFtrace(Ftrace)

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushQuaternion(![Quaternion](Type-Quaternion.png "Quaternion"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushStcontrol(Stcontrol)

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushMatrix4(![Matrix4](Type-Matrix4.png "Matrix4"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushBone(![Bone](Type-Bone.png "Bone"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushVector(![Vector](Type-Vector.png "Vector"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushMatrix(![Matrix](Type-Matrix.png "Matrix"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushMatrix2(![Matrix4](Type-Matrix2.png "Matrix2"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushAngle(![Angle](Type-Angle.png "Angle"))

Adds the variable to the end of the table (10 ops)

### ![Table](Type-Table.png "Table"):pushEntity(![Entity](Type-Entity.png "Entity"))

Adds the variable to the end of the table (10 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ![Table](Type-Table.png "Table"):popWirelink()

Removes and returns the last variable (10 ops)

### ![String](Type-String.png "String") = ![Table](Type-Table.png "Table"):popString()

Removes and returns the last variable (10 ops)

### Stcontrol = ![Table](Type-Table.png "Table"):popStcontrol()

Removes and returns the last variable (10 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ![Table](Type-Table.png "Table"):popMatrix4()

Removes and returns the last variable (10 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ![Table](Type-Table.png "Table"):popQuaternion()

Removes and returns the last variable (10 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ![Table](Type-Table.png "Table"):popMatrix2()

Removes and returns the last variable (10 ops)

### ![Bone](Type-Bone.png "Bone") = ![Table](Type-Table.png "Table"):popBone()

Removes and returns the last variable (10 ops)

### Tracedata = ![Table](Type-Table.png "Table"):popTracedata()

Removes and returns the last variable (10 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ![Table](Type-Table.png "Table"):popComplex()

Removes and returns the last variable (10 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ![Table](Type-Table.png "Table"):popMatrix()

Removes and returns the last variable (10 ops)

### Effect = ![Table](Type-Table.png "Table"):popEffect()

Removes and returns the last variable (10 ops)

### ![Vector](Type-Vector.png "Vector") = ![Table](Type-Table.png "Table"):popVector()

Removes and returns the last variable (10 ops)

### ![Angle](Type-Angle.png "Angle") = ![Table](Type-Table.png "Table"):popAngle()

Removes and returns the last variable (10 ops)

### ![Entity](Type-Entity.png "Entity") = ![Table](Type-Table.png "Table"):popEntity()

Removes and returns the last variable (10 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ![Table](Type-Table.png "Table"):popRanger()

Removes and returns the last variable (10 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Table](Type-Table.png "Table"):popVector4()

Removes and returns the last variable (10 ops)

### ![Table](Type-Table.png "Table") = ![Table](Type-Table.png "Table"):popTable()

Removes and returns the last variable (10 ops)

### ![Array](Type-Array.png "Array") = ![Table](Type-Table.png "Table"):popArray()

Removes and returns the last variable (10 ops)

### ![Number](Type-Number.png "Number") = ![Table](Type-Table.png "Table"):popNumber()

Removes and returns the last variable (10 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Table](Type-Table.png "Table"):popVector2()

Removes and returns the last variable (10 ops)

### Ftrace = ![Table](Type-Table.png "Table"):popFtrace()

Removes and returns the last variable (10 ops)

### ![Table](Type-Table.png "Table"):insertVector2(![Number](Type-Number.png "Number"), ![Vector2](Type-Vector2.png "Vector2"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertBone(![Number](Type-Number.png "Number"), ![Bone](Type-Bone.png "Bone"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertMatrix2(![Number](Type-Number.png "Number"), ![Matrix4](Type-Matrix2.png "Matrix2"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertFtrace(![Number](Type-Number.png "Number"), Ftrace)

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertVector4(![Number](Type-Number.png "Number"), ![Vector4](Type-Vector4.png "Vector4"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertMatrix(![Number](Type-Number.png "Number"), ![Matrix](Type-Matrix.png "Matrix"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertQuaternion(![Number](Type-Number.png "Number"), ![Quaternion](Type-Quaternion.png "Quaternion"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertTable(![Number](Type-Number.png "Number"), ![Table](Type-Table.png "Table"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertAngle(![Number](Type-Number.png "Number"), ![Angle](Type-Angle.png "Angle"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertVector(![Number](Type-Number.png "Number"), ![Vector](Type-Vector.png "Vector"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertNumber(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertWirelink(![Number](Type-Number.png "Number"), ![WireLink](Type-WireLink.png "WireLink"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertEffect(![Number](Type-Number.png "Number"), Effect)

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertTracedata(![Number](Type-Number.png "Number"), Tracedata)

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertStcontrol(![Number](Type-Number.png "Number"), Stcontrol)

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertEntity(![Number](Type-Number.png "Number"), ![Entity](Type-Entity.png "Entity"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertMatrix4(![Number](Type-Number.png "Number"), ![Matrix4](Type-Matrix4.png "Matrix4"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertComplex(![Number](Type-Number.png "Number"), ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertRanger(![Number](Type-Number.png "Number"), ![RangerData](Type-RangerData.png "RangerData"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertString(![Number](Type-Number.png "Number"), ![String](Type-String.png "String"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):insertArray(![Number](Type-Number.png "Number"), ![Array](Type-Array.png "Array"))

Inserts the variable at the specified position. Moves all other indexes up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftArray(![Array](Type-Array.png "Array"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftMatrix(![Matrix](Type-Matrix.png "Matrix"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftVector4(![Vector4](Type-Vector4.png "Vector4"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftTracedata(Tracedata)

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftEntity(![Entity](Type-Entity.png "Entity"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftVector(![Vector](Type-Vector.png "Vector"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftAngle(![Angle](Type-Angle.png "Angle"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftMatrix4(![Matrix4](Type-Matrix4.png "Matrix4"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftString(![String](Type-String.png "String"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftMatrix2(![Matrix4](Type-Matrix2.png "Matrix2"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftNumber(![Number](Type-Number.png "Number"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftBone(![Bone](Type-Bone.png "Bone"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftFtrace(Ftrace)

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftVector2(![Vector2](Type-Vector2.png "Vector2"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftComplex(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftRanger(![RangerData](Type-RangerData.png "RangerData"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftStcontrol(Stcontrol)

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftWirelink(![WireLink](Type-WireLink.png "WireLink"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftTable(![Table](Type-Table.png "Table"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftEffect(Effect)

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)

### ![Table](Type-Table.png "Table"):unshiftQuaternion(![Quaternion](Type-Quaternion.png "Quaternion"))

Adds the data to the beginning of the table. Will move all other entries up one step to compensate (10 ops)