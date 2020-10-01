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

# Bone

### ![Bone](Type-Bone.png "Bone") = ![Entity](Type-Entity.png "Entity"):bone(![Number](Type-Number.png "Number") Index)

Returns Es Nth bone (3 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):bones()

Returns an array containing all of Es bones. This array's first element has the index 0! (3 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):boneCount()

Returns Es number of bones (3 ops)

### ![Bone](Type-Bone.png "Bone") = nobone()

Returns an invalid bone (1 ops)

### ![Entity](Type-Entity.png "Entity") = ![Bone](Type-Bone.png "Bone"):entity()

Returns the entity B belongs to (1 ops)

### ![Number](Type-Number.png "Number") = ![Bone](Type-Bone.png "Bone"):index()

Returns Bs index in the entity it belongs to. Returns -1 if the bone is invalid or an error occured (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):pos()

Returns Bs position (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):forward()

Returns a vector describing Bs forward direction (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):right()

Returns a vector describing Bs right direction (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):up()

Returns a vector describing Bs up direction (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):vel()

Returns Bs velocity (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):velL()

Returns Bs velocity in local coordinates (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):toWorld(![Vector](Type-Vector.png "Vector") Pos)

Transforms V from local coordinates (as seen from B) to world coordinates (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):toLocal(![Vector](Type-Vector.png "Vector") Pos)

Transforms V from world coordinates to local coordinates (as seen from B) (1 ops)

### ![Angle](Type-Angle.png "Angle") = ![Bone](Type-Bone.png "Bone"):angVel()

Returns Bs angular velocity (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):angVelVector()

Returns rotation axis, velocity and direction given as the vector's direction, magnitude and sense (1 ops)

### ![Angle](Type-Angle.png "Angle") = ![Bone](Type-Bone.png "Bone"):angles()

Returns Bs pitch, yaw and roll angles (1 ops)

### ![Number](Type-Number.png "Number") = ![Bone](Type-Bone.png "Bone"):bearing(![Vector](Type-Vector.png "Vector") Pos)

Gets the bearing from the bone to the vector (1 ops)

### ![Number](Type-Number.png "Number") = ![Bone](Type-Bone.png "Bone"):elevation(![Vector](Type-Vector.png "Vector") Pos)

Gets the elevation from the bone to the vector (1 ops)

### ![Angle](Type-Angle.png "Angle") = ![Bone](Type-Bone.png "Bone"):heading(![Vector](Type-Vector.png "Vector") Pos)

Gets the elevation and bearing from the bone to the vector (1 ops)

### ![Number](Type-Number.png "Number") = ![Bone](Type-Bone.png "Bone"):mass()

Returns Bs mass (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):massCenter()

Returns Bs Center of Mass (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):massCenterL()

Returns Bs Center of Mass in local coordinates (1 ops)

### ![Bone](Type-Bone.png "Bone"):setMass(![Number](Type-Number.png "Number") Mass)

Sets the mass of the bone (between 0.001 and 50,000) (1 ops)

### ![Vector](Type-Vector.png "Vector") = ![Bone](Type-Bone.png "Bone"):inertia()

Gets the principal components of Bs inertia tensor in the form vec(Ixx, Iyy, Izz) (1 ops)

### ![Bone](Type-Bone.png "Bone"):applyForce(![Vector](Type-Vector.png "Vector") Force)

Applies force to the bone according to the given vector's direction and magnitude (30 ops)

### ![Bone](Type-Bone.png "Bone"):applyOffsetForce(![Vector](Type-Vector.png "Vector") Force, ![Vector](Type-Vector.png "Vector") Pos)

Applies force to the bone according to the first vector from the location of the second (30 ops)

### ![Bone](Type-Bone.png "Bone"):applyAngForce(![Angle](Type-Angle.png "Angle") Angforce)

Applies torque to the bone according to the given angle (30 ops)

### ![Bone](Type-Bone.png "Bone"):applyTorque(![Vector](Type-Vector.png "Vector") Torque)

Applies torque to the bone according to the given vector, representing the torque axis, magnitude and direction (30 ops)

### ![Number](Type-Number.png "Number") = ![Bone](Type-Bone.png "Bone"):isFrozen()

Returns 1 if B is frozen, 0 otherwise (2 ops)

### ![String](Type-String.png "String") = toString(![Bone](Type-Bone.png "Bone") B)

Converts bone to string (2 ops)