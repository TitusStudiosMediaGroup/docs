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

# Complex

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = comp()

Returns complex zero (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = comp(![Number](Type-Number.png "Number") A)

Converts a real number to complex (returns complex number with real part N and imaginary part 0) (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = comp(![Number](Type-Number.png "Number") A, ![Number](Type-Number.png "Number") B)

Returns a + b*i (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = i()

Returns the imaginary unit i (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = i(![Number](Type-Number.png "Number") B)

Returns N*i (2 ops)

### ![Number](Type-Number.png "Number") = abs(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Returns the absolute value of C (2 ops)

### ![Number](Type-Number.png "Number") = arg(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Returns the argument of C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = conj(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Returns the conjugate of C (2 ops)

### ![Number](Type-Number.png "Number") = real(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Returns the real part of C (2 ops)

### ![Number](Type-Number.png "Number") = imag(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Returns the imaginary part of C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = exp(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Raises Euler's constant e to the power of C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = log(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the natural logarithm of C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = log(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Base, ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the logarithm of C2 to a complex base C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = log(![Number](Type-Number.png "Number") Base, ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the logarithm of C to a real base N (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = log2(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the logarithm of C to base 2 (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = log10(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the logarithm of C to base 10 (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = sqrt(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the square root of C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = csqrt(![Number](Type-Number.png "Number") N)

Calculates the complex square root of the real number N (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = sin(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the sine of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = cos(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the cosine of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = sinh(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the hyperbolic sine of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = cosh(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the hyperbolic cosine of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = tan(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the tangent of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = cot(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the cotangent of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = asin(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the inverse sine of C (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = acos(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the inverse cosine of C (5 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = atan(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the inverse tangent of C (5 ops)

### ![Number](Type-Number.png "Number") = atan2(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the principle value of C (2 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = tanh(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the hyperbolic tangent of C (4 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = coth(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the hyperbolic cotangent of C (4 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = sec(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the secant of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = csc(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the cosecant of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = sech(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the hyperbolic secant of C (3 ops)

### ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") = csch(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Calculates the hyperbolic cosecant of C (3 ops)

### ![String](Type-String.png "String") = toString(![ComplexNumber](Type-ComplexNumber.png "ComplexNumber") Z)

Formats C as a string (15 ops)

### ![String](Type-String.png "String") = ![ComplexNumber](Type-ComplexNumber.png "ComplexNumber"):toString()

The same as toString(C) (15 ops)