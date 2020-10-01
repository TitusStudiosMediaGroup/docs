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

# Wirelink

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):isHiSpeed()

Returns true if the linked component is high-speed capable (2 ops)

### ![Entity](Type-Entity.png "Entity") = ![WireLink](Type-WireLink.png "WireLink"):entity()

Returns the entity of the linked component (2 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):hasInput(![String](Type-String.png "String") Portname)

Returns true if the linked component has an input of the specified name (2 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):hasOutput(![String](Type-String.png "String") Portname)

Returns true if the linked component has an output of the specified name (2 ops)

### ![Array](Type-Array.png "Array") = ![WireLink](Type-WireLink.png "WireLink"):array(![String](Type-String.png "String"))

Returns the array from the specified address of linked component. Deprecated, use XWL[S,array] instead (5 ops)

### Gtable = ![WireLink](Type-WireLink.png "WireLink"):gtable(![String](Type-String.png "String"))

Returns the gtable from the specified address of linked component. Deprecated, use XWL[S,gtable] instead (5 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ![WireLink](Type-WireLink.png "WireLink"):matrix(![String](Type-String.png "String"))

Returns the matrix from the specified address of linked component. Deprecated, use XWL[S,matrix] instead (5 ops)

### ![Table](Type-Table.png "Table") = ![WireLink](Type-WireLink.png "WireLink"):table(![String](Type-String.png "String"))

Returns the table from the specified address of linked component. Deprecated, use XWL[S,table] instead (5 ops)

### ![Angle](Type-Angle.png "Angle") = ![WireLink](Type-WireLink.png "WireLink"):angle(![String](Type-String.png "String"))

Returns the angle from the specified address of linked component. Deprecated, use XWL[S,angle] instead (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![WireLink](Type-WireLink.png "WireLink"):vector2(![String](Type-String.png "String"))

Returns the vector2 from the specified address of linked component. Deprecated, use XWL[S,vector2] instead (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ![WireLink](Type-WireLink.png "WireLink"):complex(![String](Type-String.png "String"))

Returns the complex from the specified address of linked component. Deprecated, use XWL[S,complex] instead (5 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ![WireLink](Type-WireLink.png "WireLink"):matrix4(![String](Type-String.png "String"))

Returns the matrix4 from the specified address of linked component. Deprecated, use XWL[S,matrix4] instead (5 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ![WireLink](Type-WireLink.png "WireLink"):matrix2(![String](Type-String.png "String"))

Returns the matrix2 from the specified address of linked component. Deprecated, use XWL[S,matrix2] instead (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![WireLink](Type-WireLink.png "WireLink"):vector4(![String](Type-String.png "String"))

Returns the vector4 from the specified address of linked component. Deprecated, use XWL[S,vector4] instead (5 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ![WireLink](Type-WireLink.png "WireLink"):wirelink(![String](Type-String.png "String"))

Returns the wirelink from the specified address of linked component. Deprecated, use XWL[S,wirelink] instead (5 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ![WireLink](Type-WireLink.png "WireLink"):quaternion(![String](Type-String.png "String"))

Returns the quaternion from the specified address of linked component. Deprecated, use XWL[S,quaternion] instead (5 ops)

### ![String](Type-String.png "String") = ![WireLink](Type-WireLink.png "WireLink"):string(![String](Type-String.png "String"))

Returns the string from the specified address of linked component. Deprecated, use XWL[S,string] instead (5 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):number(![String](Type-String.png "String"))

Returns the number from the specified address of linked component. Deprecated, use XWL[S,number] instead (5 ops)

### Tracedata = ![WireLink](Type-WireLink.png "WireLink"):tracedata(![String](Type-String.png "String"))

Returns the tracedata from the specified address of linked component. Deprecated, use XWL[S,tracedata] instead (5 ops)

### ![Bone](Type-Bone.png "Bone") = ![WireLink](Type-WireLink.png "WireLink"):bone(![String](Type-String.png "String"))

Returns the bone from the specified address of linked component. Deprecated, use XWL[S,bone] instead (5 ops)

### Stcontrol = ![WireLink](Type-WireLink.png "WireLink"):stcontrol(![String](Type-String.png "String"))

Returns the stcontrol from the specified address of linked component. Deprecated, use XWL[S,stcontrol] instead (5 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ![WireLink](Type-WireLink.png "WireLink"):ranger(![String](Type-String.png "String"))

Returns the ranger from the specified address of linked component. Deprecated, use XWL[S,ranger] instead (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![WireLink](Type-WireLink.png "WireLink"):entity(![String](Type-String.png "String"))

Returns the entity from the specified address of linked component. Deprecated, use XWL[S,entity] instead (5 ops)

### Effect = ![WireLink](Type-WireLink.png "WireLink"):effect(![String](Type-String.png "String"))

Returns the effect from the specified address of linked component. Deprecated, use XWL[S,effect] instead (5 ops)

### Ftrace = ![WireLink](Type-WireLink.png "WireLink"):ftrace(![String](Type-String.png "String"))

Returns the ftrace from the specified address of linked component. Deprecated, use XWL[S,ftrace] instead (5 ops)

### ![Vector](Type-Vector.png "Vector") = ![WireLink](Type-WireLink.png "WireLink"):vector(![String](Type-String.png "String"))

Returns the vector from the specified address of linked component. Deprecated, use XWL[S,vector] instead (5 ops)

### ![Vector](Type-Vector.png "Vector") = ![WireLink](Type-WireLink.png "WireLink"):setVector(![String](Type-String.png "String"), ![Vector](Type-Vector.png "Vector"))

Sets the component's input of the specified name equal to specified vector. Deprecated, use XWL[S,vector] = X instead (5 ops)

### ![Angle](Type-Angle.png "Angle") = ![WireLink](Type-WireLink.png "WireLink"):setAngle(![String](Type-String.png "String"), ![Angle](Type-Angle.png "Angle"))

Sets the component's input of the specified name equal to specified angle. Deprecated, use XWL[S,angle] = X instead (5 ops)

### Gtable = ![WireLink](Type-WireLink.png "WireLink"):setGtable(![String](Type-String.png "String"), Gtable)

Sets the component's input of the specified name equal to specified gtable. Deprecated, use XWL[S,gtable] = X instead (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![WireLink](Type-WireLink.png "WireLink"):setEntity(![String](Type-String.png "String"), ![Entity](Type-Entity.png "Entity"))

Sets the component's input of the specified name equal to specified entity. Deprecated, use XWL[S,entity] = X instead (5 ops)

### ![String](Type-String.png "String") = ![WireLink](Type-WireLink.png "WireLink"):setString(![String](Type-String.png "String"), ![String](Type-String.png "String"))

Sets the component's input of the specified name equal to specified string. Deprecated, use XWL[S,string] = X instead (5 ops)

### ![Bone](Type-Bone.png "Bone") = ![WireLink](Type-WireLink.png "WireLink"):setBone(![String](Type-String.png "String"), ![Bone](Type-Bone.png "Bone"))

Sets the component's input of the specified name equal to specified bone. Deprecated, use XWL[S,bone] = X instead (5 ops)

### Stcontrol = ![WireLink](Type-WireLink.png "WireLink"):setStcontrol(![String](Type-String.png "String"), Stcontrol)

Sets the component's input of the specified name equal to specified stcontrol. Deprecated, use XWL[S,stcontrol] = X instead (5 ops)

### Tracedata = ![WireLink](Type-WireLink.png "WireLink"):setTracedata(![String](Type-String.png "String"), Tracedata)

Sets the component's input of the specified name equal to specified tracedata. Deprecated, use XWL[S,tracedata] = X instead (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = ![WireLink](Type-WireLink.png "WireLink"):setComplex(![String](Type-String.png "String"), ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"))

Sets the component's input of the specified name equal to specified complex. Deprecated, use XWL[S,complex] = X instead (5 ops)

### ![Matrix](Type-Matrix.png "Matrix") = ![WireLink](Type-WireLink.png "WireLink"):setMatrix(![String](Type-String.png "String"), ![Matrix](Type-Matrix.png "Matrix"))

Sets the component's input of the specified name equal to specified matrix. Deprecated, use XWL[S,matrix] = X instead (5 ops)

### Ftrace = ![WireLink](Type-WireLink.png "WireLink"):setFtrace(![String](Type-String.png "String"), Ftrace)

Sets the component's input of the specified name equal to specified ftrace. Deprecated, use XWL[S,ftrace] = X instead (5 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ![WireLink](Type-WireLink.png "WireLink"):setMatrix2(![String](Type-String.png "String"), ![Matrix4](Type-Matrix2.png "Matrix2"))

Sets the component's input of the specified name equal to specified matrix2. Deprecated, use XWL[S,matrix2] = X instead (5 ops)

### ![WireLink](Type-WireLink.png "WireLink") = ![WireLink](Type-WireLink.png "WireLink"):setWirelink(![String](Type-String.png "String"), ![WireLink](Type-WireLink.png "WireLink"))

Sets the component's input of the specified name equal to specified wirelink. Deprecated, use XWL[S,wirelink] = X instead (5 ops)

### ![Quaternion](Type-Quaternion.png "Quaternion") = ![WireLink](Type-WireLink.png "WireLink"):setQuaternion(![String](Type-String.png "String"), ![Quaternion](Type-Quaternion.png "Quaternion"))

Sets the component's input of the specified name equal to specified quaternion. Deprecated, use XWL[S,quaternion] = X instead (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![WireLink](Type-WireLink.png "WireLink"):setVector4(![String](Type-String.png "String"), ![Vector4](Type-Vector4.png "Vector4"))

Sets the component's input of the specified name equal to specified vector4. Deprecated, use XWL[S,vector4] = X instead (5 ops)

### ![Table](Type-Table.png "Table") = ![WireLink](Type-WireLink.png "WireLink"):setTable(![String](Type-String.png "String"), ![Table](Type-Table.png "Table"))

Sets the component's input of the specified name equal to specified table. Deprecated, use XWL[S,table] = X instead (5 ops)

### ![RangerData](Type-RangerData.png "RangerData") = ![WireLink](Type-WireLink.png "WireLink"):setRanger(![String](Type-String.png "String"), ![RangerData](Type-RangerData.png "RangerData"))

Sets the component's input of the specified name equal to specified ranger. Deprecated, use XWL[S,ranger] = X instead (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![WireLink](Type-WireLink.png "WireLink"):setVector2(![String](Type-String.png "String"), ![Vector2](Type-Vector2.png "Vector2"))

Sets the component's input of the specified name equal to specified vector2. Deprecated, use XWL[S,vector2] = X instead (5 ops)

### Effect = ![WireLink](Type-WireLink.png "WireLink"):setEffect(![String](Type-String.png "String"), Effect)

Sets the component's input of the specified name equal to specified effect. Deprecated, use XWL[S,effect] = X instead (5 ops)

### ![Array](Type-Array.png "Array") = ![WireLink](Type-WireLink.png "WireLink"):setArray(![String](Type-String.png "String"), ![Array](Type-Array.png "Array"))

Sets the component's input of the specified name equal to specified array. Deprecated, use XWL[S,array] = X instead (5 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ![WireLink](Type-WireLink.png "WireLink"):setMatrix4(![String](Type-String.png "String"), ![Matrix4](Type-Matrix4.png "Matrix4"))

Sets the component's input of the specified name equal to specified matrix4. Deprecated, use XWL[S,matrix4] = X instead (5 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):setNumber(![String](Type-String.png "String"), ![Number](Type-Number.png "Number"))

Sets the component's input of the specified name equal to specified number. Deprecated, use XWL[S,number] = X instead (5 ops)

### ![WireLink](Type-WireLink.png "WireLink"):setXyz(![Vector](Type-Vector.png "Vector") Value)

Sets the X/Y/Z to the corresponding values in the vector (15 ops)

### ![Vector](Type-Vector.png "Vector") = ![WireLink](Type-WireLink.png "WireLink"):xyz()

Retrieves the X/Y/Z as the corresponding values in the vector (15 ops)

### ![WireLink](Type-WireLink.png "WireLink") = wirelink()

Returns wirelink to this E2 (5 ops)

### ![WireLink](Type-WireLink.png "WireLink") = nowirelink()

Returns an invalid wirelink (1 ops)

### ![Array](Type-Array.png "Array") = ![WireLink](Type-WireLink.png "WireLink"):inputs()

Returns an array of all the inputs that XWL has without their types. Returns an empty array if it has none (15 ops)

### ![Array](Type-Array.png "Array") = ![WireLink](Type-WireLink.png "WireLink"):outputs()

Returns an array of all the outputs that XWL has without their types. Returns an empty array if it has none (15 ops)

### ![String](Type-String.png "String") = ![WireLink](Type-WireLink.png "WireLink"):inputType(![String](Type-String.png "String") Input)

Returns the type of input that S is in lowercase. ( "NORMAL" is changed to "number" ) (15 ops)

### ![String](Type-String.png "String") = ![WireLink](Type-WireLink.png "WireLink"):outputType(![String](Type-String.png "String") Output)

Returns the type of output that S is in lowercase. ( "NORMAL" is changed to "number" ) (15 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):writeCell(![Number](Type-Number.png "Number") Address, ![Number](Type-Number.png "Number") Value)

Writes value into specified memory cell. Deprecated, use XWL[N] = X instead (5 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):readCell(![Number](Type-Number.png "Number") Address)

Returns contents of the specified memory cell. Deprecated, use XWL[N] instead (5 ops)

### ![Array](Type-Array.png "Array") = ![WireLink](Type-WireLink.png "WireLink"):readArray(![Number](Type-Number.png "Number") Start, ![Number](Type-Number.png "Number") Size)

Reads an array's elements from a piece of memory. Strings and sub-tables (angles, vectors, matrices) are written as pointers to the actual data. Strings are written null-terminated (5 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Number](Type-Number.png "Number") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeString(snnvn), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeString(snnnv), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeString(snnvv), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Number](Type-Number.png "Number") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeString(snnnn), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor)

Same as XWL:writeString(snnv), with an extra argument for background colour (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor)

Same as XWL:writeString(snnn), with an extra argument for background colour (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Number](Type-Number.png "Number") Bgcolor)

Same as XWL:writeString(snnv), with an extra argument for background colour. This is in the form of a 3-digit RGB code. 0 is black, while 999 is white, 900 is pure red and so on (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Number](Type-Number.png "Number") Bgcolor)

Same as XWL:writeString(snnn), with an extra argument for background colour. 3-digit RGB again (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor)

Same as XWL:writeString(snn), with an extra argument for the text colour (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor)

Same as XWL:writeString(snn), with an extra argument for the text colour. This is in the form of a 3-digit RGB code. 0 is black, while 999 is white, 900 is pure red and so on (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y)

A helper function for using the Wired Console Screen. The string will be written to the screen in white text on black background. The number arguments specify the starting position - X/Horizontal (0-29 recommended) and Y/vertical (0-17) (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Number](Type-Number.png "Number") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeUnicodeString(snnvn), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Number](Type-Number.png "Number") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeUnicodeString(snnnn), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeUnicodeString(snnnv), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor, ![Number](Type-Number.png "Number") Flash)

Same as XWL:writeUnicodeString(snnvv), with an extra argument for flashing text. 0 or 1 is recommended (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Number](Type-Number.png "Number") Bgcolor)

Same as XWL:writeUnicodeString(snnn), with an extra argument for background colour. 3-digit RGB again (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor)

Same as XWL:writeUnicodeString(snnv), with an extra argument for background colour (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor, ![Vector](Type-Vector.png "Vector") Bgcolor)

Same as XWL:writeUnicodeString(snnn), with an extra argument for background colour (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor, ![Number](Type-Number.png "Number") Bgcolor)

Same as XWL:writeUnicodeString(snnv), with an extra argument for background colour. This is in the form of a 3-digit RGB code. 0 is black, while 999 is white, 900 is pure red and so on (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Vector](Type-Vector.png "Vector") Textcolor)

Same as XWL:writeUnicodeString(snn), with an extra argument for the text colour (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y, ![Number](Type-Number.png "Number") Textcolor)

Same as XWL:writeUnicodeString(snn), with an extra argument for the text colour. This is in the form of a 3-digit RGB code. 0 is black, while 999 is white, 900 is pure red and so on (20 ops)

### ![WireLink](Type-WireLink.png "WireLink"):writeUnicodeString(![String](Type-String.png "String") Text, ![Number](Type-Number.png "Number") X, ![Number](Type-Number.png "Number") Y)

A helper function for using the Wired Console Screen. The unicode string will be written to the screen in white text on black background. The number arguments specify the starting position - X/Horizontal (0-29 recommended) and Y/vertical (0-17) (20 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):writeString(![Number](Type-Number.png "Number") Address, ![String](Type-String.png "String") Data)

Writes a null-terminated string to the given address. Returns the next free address or 0 on failure (20 ops)

### ![String](Type-String.png "String") = ![WireLink](Type-WireLink.png "WireLink"):readString(![Number](Type-Number.png "Number") Address)

Reads a null-terminated string from the given address. Returns an empty string on failure (20 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):writeArray(![Number](Type-Number.png "Number") Address, ![Array](Type-Array.png "Array") Data)

Writes an array's elements into a piece of memory. Strings and sub-tables (angles, vectors, matrices) are written as pointers to the actual data. Strings are written null-terminated (20 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):writeTable(![Number](Type-Number.png "Number") Address, ![Table](Type-Table.png "Table") Data)

Same as writeArray, except it uses the numerically indexed variables of the table instead (20 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):writeArraySimple(![Number](Type-Number.png "Number") Address, ![Array](Type-Array.png "Array") Data)

 (20 ops)

### ![Number](Type-Number.png "Number") = ![WireLink](Type-WireLink.png "WireLink"):writeTableSimple(![Number](Type-Number.png "Number") Address, ![Table](Type-Table.png "Table") Data)

 (20 ops)