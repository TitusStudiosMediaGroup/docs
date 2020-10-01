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

# Selfaware

### ![Entity](Type-Entity.png "Entity") = entity()

Gets the entity of the expression (1 ops)

### ![Entity](Type-Entity.png "Entity") = owner()

Gets the owner of the expression ( same as entity():owner() ) (1 ops)

### selfDestruct()

Removes the expression (5 ops)

### selfDestructAll()

Removes the expression and all constrained props (5 ops)

### ![Array](Type-Array.png "Array") = ioOutputEntities(![String](Type-String.png "String") Output)

Returns an array of all entities wired to the output S (10 ops)

### ![Entity](Type-Entity.png "Entity") = ioInputEntity(![String](Type-String.png "String") Input)

Returns the entity the input S is wired to (10 ops)

### ![Vector](Type-Vector.png "Vector") = ioSetOutput(![String](Type-String.png "String"), ![Vector](Type-Vector.png "Vector"))

Trigger the output S of the E2 with the vector value (5 ops)

### ![Array](Type-Array.png "Array") = ioSetOutput(![String](Type-String.png "String"), ![Array](Type-Array.png "Array"))

Trigger the output S of the E2 with the array value (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ioSetOutput(![String](Type-String.png "String"), ![Vector4](Type-Vector4.png "Vector4"))

Trigger the output S of the E2 with the vector4 value (5 ops)

### ![Angle](Type-Angle.png "Angle") = ioSetOutput(![String](Type-String.png "String"), ![Angle](Type-Angle.png "Angle"))

Trigger the output S of the E2 with the angle value (5 ops)

### ![Number](Type-Number.png "Number") = ioSetOutput(![String](Type-String.png "String"), ![Number](Type-Number.png "Number"))

Trigger the output S of the E2 with the number value (5 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ioSetOutput(![String](Type-String.png "String"), ![Quaternion](Type-Quaternion.png "Quaternion"))

Trigger the output S of the E2 with the quaternion value (5 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ioSetOutput(![String](Type-String.png "String"), ![Matrix4](Type-Matrix2.png "Matrix2"))

Trigger the output S of the E2 with the matrix2 value (5 ops)

### Ftrace = ioSetOutput(![String](Type-String.png "String"), Ftrace)

Trigger the output S of the E2 with the ftrace value (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ioSetOutput(![String](Type-String.png "String"), ![Vector2](Type-Vector2.png "Vector2"))

Trigger the output S of the E2 with the vector2 value (5 ops)

### ![Table](Type-Table.png "Table") = ioSetOutput(![String](Type-String.png "String"), ![Table](Type-Table.png "Table"))

Trigger the output S of the E2 with the table value (5 ops)

### Tracedata = ioSetOutput(![String](Type-String.png "String"), Tracedata)

Trigger the output S of the E2 with the tracedata value (5 ops)

### Stcontrol = ioSetOutput(![String](Type-String.png "String"), Stcontrol)

Trigger the output S of the E2 with the stcontrol value (5 ops)

### Effect = ioSetOutput(![String](Type-String.png "String"), Effect)

Trigger the output S of the E2 with the effect value (5 ops)

### ![Entity](Type-Entity.png "Entity") = ioSetOutput(![String](Type-String.png "String"), ![Entity](Type-Entity.png "Entity"))

Trigger the output S of the E2 with the entity value (5 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ioSetOutput(![String](Type-String.png "String"), ![Matrix](Type-Matrix.png "Matrix"))

Trigger the output S of the E2 with the matrix value (5 ops)

### ![Bone](Type-Bone.png "Bone") = ioSetOutput(![String](Type-String.png "String"), ![Bone](Type-Bone.png "Bone"))

Trigger the output S of the E2 with the bone value (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ioSetOutput(![String](Type-String.png "String"), ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"))

Trigger the output S of the E2 with the complex value (5 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ioSetOutput(![String](Type-String.png "String"), ![RangerData](Type-RangerData.png "RangerData"))

Trigger the output S of the E2 with the ranger value (5 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ioSetOutput(![String](Type-String.png "String"), ![WireLink](Type-WireLink.png "WireLink"))

Trigger the output S of the E2 with the wirelink value (5 ops)

### ![String](Type-String.png "String") = ioSetOutput(![String](Type-String.png "String"), ![String](Type-String.png "String"))

Trigger the output S of the E2 with the string value (5 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ioSetOutput(![String](Type-String.png "String"), ![Matrix4](Type-Matrix4.png "Matrix4"))

Trigger the output S of the E2 with the matrix4 value (5 ops)

### ![Angle](Type-Angle.png "Angle") = ioGetInputAngle(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Array](Type-Array.png "Array") = ioGetInputArray(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Entity](Type-Entity.png "Entity") = ioGetInputEntity(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ioGetInputQuaternion(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ioGetInputVector2(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ioGetInputMatrix(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### Tracedata = ioGetInputTracedata(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### Stcontrol = ioGetInputStcontrol(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ioGetInputRanger(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Bone](Type-Bone.png "Bone") = ioGetInputBone(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ioGetInputComplex(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![String](Type-String.png "String") = ioGetInputString(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ioGetInputMatrix2(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### Ftrace = ioGetInputFtrace(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ioGetInputMatrix4(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ioGetInputWirelink(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Number](Type-Number.png "Number") = ioGetInputNumber(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Table](Type-Table.png "Table") = ioGetInputTable(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ioGetInputVector4(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### ![Vector](Type-Vector.png "Vector") = ioGetInputVector(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### Effect = ioGetInputEffect(![String](Type-String.png "String"))

Get the value of the input S of the E2 (5 ops)

### setName(![String](Type-String.png "String") Name)

Set the name of the E2 (5 ops)

### ![Entity](Type-Entity.png "Entity"):setName(![String](Type-String.png "String") Name)

Set the name of another E2 or component name for other entities (5 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):getName()

Get the name of another E2, compatible entity or wiremod component name (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Number](Type-Number.png "Number") Value)

 (1 ops)

### ![Number](Type-Number.png "Number") = changed(![String](Type-String.png "String"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Bone](Type-Bone.png "Bone"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![WireLink](Type-WireLink.png "WireLink"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Entity](Type-Entity.png "Entity"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Vector](Type-Vector.png "Vector") Value)

 (1 ops)

### ![Number](Type-Number.png "Number") = changed(![Angle](Type-Angle.png "Angle") Value)

 (1 ops)

### ![Number](Type-Number.png "Number") = changed(![Matrix](Type-Matrix.png "Matrix"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Vector4](Type-Vector4.png "Vector4"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![RangerData](Type-RangerData.png "RangerData"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Matrix4](Type-Matrix4.png "Matrix4"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Quaternion](Type-Quaternion.png "Quaternion"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(Stcontrol)

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(Ftrace)

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Matrix4](Type-Matrix2.png "Matrix2"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(Effect)

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(Tracedata)

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(Gtable)

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"))

 (5 ops)

### ![Number](Type-Number.png "Number") = changed(![Vector2](Type-Vector2.png "Vector2"))

 (5 ops)

### ![Number](Type-Number.png "Number") = hash()

Returns a numerical hash using the code of the E2 itself (Including comments) (5 ops)

### ![Number](Type-Number.png "Number") = hashNoComments()

Returns a numerical hash using the code of the E2 itself (Excluding comments) (5 ops)

### ![Number](Type-Number.png "Number") = hash(![String](Type-String.png "String") Str)

Returns a numerical hash using the string specified (5 ops)