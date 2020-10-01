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

# Vector2

### ![Vector2](Type-Vector2.png "Vector2") = vec2()

Same as vec2(0,0) (1 ops)

### ![Vector2](Type-Vector2.png "Vector2") = vec2(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Makes a 2D vector (2 ops)

### ![Vector2](Type-Vector2.png "Vector2") = vec2(![Number](Type-Number.png "Number"))

Makes a 2D vector (2 ops)

### ![Vector2](Type-Vector2.png "Vector2") = vec2(![Vector](Type-Vector.png "Vector"))

Converts a 3D vector into a 2D vector (the z component is dropped) (2 ops)

### ![Vector2](Type-Vector2.png "Vector2") = vec2(![Vector4](Type-Vector4.png "Vector4"))

Converts a 4D vector into a 2D vector (the z and w components are dropped) (2 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):length()

Gets the length of the vector (3 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):length2()

Gets the squared length of the vector (3 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):distance(![Vector2](Type-Vector2.png "Vector2"))

Gets the distance between 2D vectors (3 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):distance2(![Vector2](Type-Vector2.png "Vector2"))

Gets the squared distance between 2D vectors (3 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Vector2](Type-Vector2.png "Vector2"):normalized()

Gets the normalized vector (3 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):dot(![Vector2](Type-Vector2.png "Vector2"))

Gets the 2D vector dot (scalar) product (3 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):cross(![Vector2](Type-Vector2.png "Vector2"))

Gets the 2D vector cross product/wedge product (3 ops)

### ![Matrix4](Type-Matrix2.png "Matrix2") = ![Vector2](Type-Vector2.png "Vector2"):outerProduct(![Vector2](Type-Vector2.png "Vector2"))

Gets the outer product (tensor product) and returns a matrix (tensor) (3 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Vector2](Type-Vector2.png "Vector2"):rotate(![Number](Type-Number.png "Number"))

Rotates a vector by the argument (given in degrees) (3 ops)

### ![Vector2](Type-Vector2.png "Vector2") = positive(![Vector2](Type-Vector2.png "Vector2"))

Returns a vector containing the positive value of each vector component, equivalent to abs(N) (3 ops)

### ![Vector2](Type-Vector2.png "Vector2") = toRad(![Vector2](Type-Vector2.png "Vector2") Xv2)

Converts the vector's magnitude from radians to radians (2 ops)

### ![Vector2](Type-Vector2.png "Vector2") = toDeg(![Vector2](Type-Vector2.png "Vector2") Xv2)

Converts the vector's magnitude from radians to degrees (2 ops)

### ![Vector2](Type-Vector2.png "Vector2") = clamp(![Vector2](Type-Vector2.png "Vector2") Input, ![Number](Type-Number.png "Number") Min, ![Number](Type-Number.png "Number") Max)

Returns a vector in the same direction as vector 1, with length clamped between argument 2(min) and argument 3(max) (3 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):x()

Gets the x component of the vector (1 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):y()

Gets the y component of the vector (1 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Vector2](Type-Vector2.png "Vector2"):setX(![Number](Type-Number.png "Number"))

Returns a copy of the 2D vector with X replaced (use as Vec2 = Vec2:setX(...)) (1 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ![Vector2](Type-Vector2.png "Vector2"):setY(![Number](Type-Number.png "Number"))

Returns a copy of the 2D vector with Y replaced (use as Vec2 = Vec2:setY(...)) (1 ops)

### ![Vector2](Type-Vector2.png "Vector2") = round(![Vector2](Type-Vector2.png "Vector2") Rv1)

Rounds XY to the nearest integer (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = round(![Vector2](Type-Vector2.png "Vector2") Rv1, ![Number](Type-Number.png "Number") Decimals)

Rounds XY to argument 2's decimal precision (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ceil(![Vector2](Type-Vector2.png "Vector2") Rv1)

Rounds XY up to the nearest integer (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = ceil(![Vector2](Type-Vector2.png "Vector2") Rv1, ![Number](Type-Number.png "Number") Decimals)

Rounds XY up to argument 2's decimal precision (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = floor(![Vector2](Type-Vector2.png "Vector2") Rv1)

Rounds XY down to the nearest integer (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = floor(![Vector2](Type-Vector2.png "Vector2") Rv1, ![Number](Type-Number.png "Number") Decimals)

Rounds XY down to argument 2's decimal precision (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = min(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Returns the vector with the smallest length (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = max(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Returns the vector with the greatest length (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = maxVec(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Returns the vector combining the highest value components of V1 and V2 (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = minVec(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Returns a vector combining the lowest value components of V1 and V2 (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = mod(![Vector2](Type-Vector2.png "Vector2"), ![Number](Type-Number.png "Number"))

Returns the remainder after XY have been divided by argument 2 (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = mod(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Returns the remainder after the components of vector 1 have been divided by the components of vector 2 (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = clamp(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Clamps vector 1's XY between the XY of vector 2(min) and vector 3(max) (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = mix(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"), ![Number](Type-Number.png "Number"))

Combines vector 1's XY with vector 2's XY by a proportion given by argument 3 (between 0 and 1) (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = bezier(![Vector2](Type-Vector2.png "Vector2") Startvec, ![Vector2](Type-Vector2.png "Vector2") Control, ![Vector2](Type-Vector2.png "Vector2") Endvec, ![Number](Type-Number.png "Number") Ratio)

Returns the 2D position on the bezier curve between the starting and ending 2D vector, given by the ratio (value between 0 and 1) (4 ops)

### ![Vector2](Type-Vector2.png "Vector2") = shift(![Vector2](Type-Vector2.png "Vector2"))

Swaps the vector's x,y components (2 ops)

### ![Number](Type-Number.png "Number") = inrange(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Returns 1 if each component of V is between (or is equal to) the components of Vmin and Vmax (2 ops)

### ![Number](Type-Number.png "Number") = ![Vector2](Type-Vector2.png "Vector2"):toAngle()

Returns the 2D angle of the vector (given in degrees, -180 to 180) (2 ops)

### ![String](Type-String.png "String") = toString(![Vector2](Type-Vector2.png "Vector2") V)

Gets the vector nicely formatted as a string "[X,Y]" (5 ops)

### ![String](Type-String.png "String") = ![Vector2](Type-Vector2.png "Vector2"):toString()

Gets the vector nicely formatted as a string "[X,Y]" (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = randvec2()

Returns a uniformly distributed, random, normalized direction vector (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = randvec2(![Number](Type-Number.png "Number") Min, ![Number](Type-Number.png "Number") Max)

Returns a random vector with its components between N1 and N2 (5 ops)

### ![Vector2](Type-Vector2.png "Vector2") = randvec2(![Vector2](Type-Vector2.png "Vector2") Min, ![Vector2](Type-Vector2.png "Vector2") Max)

Returns a random vector between V1 and V2 (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4()

Same as vec4(0,0,0,0) (1 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Number](Type-Number.png "Number"))

Makes a 4D vector (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Makes a 4D vector (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Vector2](Type-Vector2.png "Vector2"))

Converts a 2D vector into a 4D vector (the z and w components are set to 0) (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Vector2](Type-Vector2.png "Vector2"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Converts a 2D vector into a 4D vector (the z and w components are set to the second and third arguments) (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Vector2](Type-Vector2.png "Vector2"), ![Vector2](Type-Vector2.png "Vector2"))

Creates a 4D vector from two 2D vectors (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Vector](Type-Vector.png "Vector"))

Converts a 3D vector into a 4D vector (the w component is set to 0) (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = vec4(![Vector](Type-Vector.png "Vector"), ![Number](Type-Number.png "Number"))

Converts a 3D vector into a 4D vector (the w component is set to the second argument) (4 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):length()

Gets the length of the vector (7 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):length2()

Gets the squared length of the vector (7 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):distance(![Vector4](Type-Vector4.png "Vector4"))

Gets the distance between 4D vectors (7 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):distance2(![Vector4](Type-Vector4.png "Vector4"))

Gets the squared distance between 4D vectors (7 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):dot(![Vector4](Type-Vector4.png "Vector4"))

Gets the 4D vector dot (scalar) product (7 ops)

### ![Matrix4](Type-Matrix4.png "Matrix4") = ![Vector4](Type-Vector4.png "Vector4"):outerProduct(![Vector4](Type-Vector4.png "Vector4"))

Gets the outer product (tensor product) and returns a matrix (tensor) (15 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Vector4](Type-Vector4.png "Vector4"):normalized()

Gets the normalized vector (7 ops)

### ![Vector](Type-Vector.png "Vector") = ![Vector4](Type-Vector4.png "Vector4"):dehomogenized()

Converts a 3D homogeneous vector (x,y,z,w) into a 3D cartesian vector (3 ops)

### ![Vector4](Type-Vector4.png "Vector4") = positive(![Vector4](Type-Vector4.png "Vector4"))

Returns a vector containing the positive value of each vector component, equivalent to abs(N) (4 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):x()

Gets the x component of the vector (2 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):y()

Gets the y component of the vector (2 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):z()

Gets the z component of the vector (2 ops)

### ![Number](Type-Number.png "Number") = ![Vector4](Type-Vector4.png "Vector4"):w()

Gets the w component of the vector (2 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Vector4](Type-Vector4.png "Vector4"):setX(![Number](Type-Number.png "Number"))

Returns a copy of the 4D vector with X replaced (use as Vec4 = Vec4:setX(...)) (3 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Vector4](Type-Vector4.png "Vector4"):setY(![Number](Type-Number.png "Number"))

Returns a copy of the 4D vector with Y replaced (use as Vec4 = Vec4:setY(...)) (3 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Vector4](Type-Vector4.png "Vector4"):setZ(![Number](Type-Number.png "Number"))

Returns a copy of the 4D vector with Z replaced (use as Vec4 = Vec4:setZ(...)) (3 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ![Vector4](Type-Vector4.png "Vector4"):setW(![Number](Type-Number.png "Number"))

Returns a copy of the 4D vector with W replaced (use as Vec4 = Vec4:setW(...)) (3 ops)

### ![Vector4](Type-Vector4.png "Vector4") = round(![Vector4](Type-Vector4.png "Vector4") Rv1)

Rounds XYZW to the nearest integer (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = round(![Vector4](Type-Vector4.png "Vector4") Rv1, ![Number](Type-Number.png "Number") Decimals)

Rounds XYZW to argument 2's decimal precision (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ceil(![Vector4](Type-Vector4.png "Vector4") Rv1)

Rounds XYZW up to the nearest integer (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = ceil(![Vector4](Type-Vector4.png "Vector4") Rv1, ![Number](Type-Number.png "Number") Decimals)

Rounds XYZW up to argument 2's decimal precision (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = floor(![Vector4](Type-Vector4.png "Vector4") Rv1)

Rounds XYZW down to the nearest integer (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = floor(![Vector4](Type-Vector4.png "Vector4") Rv1, ![Number](Type-Number.png "Number") Decimals)

Rounds XYZW down to argument 2's decimal precision (8 ops)

### ![Vector4](Type-Vector4.png "Vector4") = min(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Returns the vector with the smallest length (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = max(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Returns the vector with the greatest length (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = maxVec(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Returns the vector combining the highest value components of V1 and V2 (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = minVec(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Returns a vector combining the lowest value components of V1 and V2 (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = mod(![Vector4](Type-Vector4.png "Vector4"), ![Number](Type-Number.png "Number"))

Returns the remainder after XYZW have been divided by argument 2 (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = mod(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Returns the remainder after the components of vector 1 have been divided by the components of vector 2 (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = clamp(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Clamps vector 1's XYZW between the XYZW of vector 2(min) and vector 3(max) (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = clamp(![Vector4](Type-Vector4.png "Vector4") Input, ![Number](Type-Number.png "Number") Min, ![Number](Type-Number.png "Number") Max)

Returns a vector in the same direction as vector 1, with length clamped between argument 2(min) and argument 3(max) (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = mix(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"), ![Number](Type-Number.png "Number"))

Combines vector 1's XYZW with vector 2's XYZW by a proportion given by argument 3 (between 0 and 1) (13 ops)

### ![Vector4](Type-Vector4.png "Vector4") = shiftR(![Vector4](Type-Vector4.png "Vector4"))

Shifts the vector's components right: shiftR( x,y,z,w ) = ( w,x,y,z ) (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = shiftL(![Vector4](Type-Vector4.png "Vector4"))

Shifts the vector's components left: shiftL( x,y,z,w ) = ( y,z,w,x ) (4 ops)

### ![Number](Type-Number.png "Number") = inrange(![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"), ![Vector4](Type-Vector4.png "Vector4"))

Returns 1 if each component of V is between (or is equal to) the components of Vmin and Vmax (4 ops)

### ![Vector4](Type-Vector4.png "Vector4") = toRad(![Vector4](Type-Vector4.png "Vector4") Xv4)

Converts the vector's magnitude from radians to radians (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = toDeg(![Vector4](Type-Vector4.png "Vector4") Xv4)

Converts the vector's magnitude from radians to degrees (5 ops)

### ![Vector4](Type-Vector4.png "Vector4") = randvec4()

Returns a uniformly distributed, random, normalized direction vector (7 ops)

### ![Vector4](Type-Vector4.png "Vector4") = randvec4(![Number](Type-Number.png "Number") Min, ![Number](Type-Number.png "Number") Max)

Returns a random vector with its components between N1 and N2 (7 ops)

### ![Vector4](Type-Vector4.png "Vector4") = randvec4(![Vector4](Type-Vector4.png "Vector4") Min, ![Vector4](Type-Vector4.png "Vector4") Max)

Returns a random vector between V1 and V2 (7 ops)

### ![String](Type-String.png "String") = ![Vector4](Type-Vector4.png "Vector4"):toString()

Gets the vector nicely formatted as a string "[X,Y,Z,W]" (7 ops)

### ![String](Type-String.png "String") = toString(![Vector4](Type-Vector4.png "Vector4") V)

Gets the vector nicely formatted as a string "[X,Y,Z,W]" (7 ops)