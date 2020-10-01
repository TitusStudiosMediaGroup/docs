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

# Number

### ![Number](Type-Number.png "Number") = min(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the lowest value Argument (1 ops)

### ![Number](Type-Number.png "Number") = min(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the lowest value Argument (1 ops)

### ![Number](Type-Number.png "Number") = min(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the lowest value Argument (1 ops)

### ![Number](Type-Number.png "Number") = max(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the highest value Argument (1 ops)

### ![Number](Type-Number.png "Number") = max(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the highest value Argument (1 ops)

### ![Number](Type-Number.png "Number") = max(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the highest value Argument (1 ops)

### ![Number](Type-Number.png "Number") = isfinite(![Number](Type-Number.png "Number") Value)

 (2 ops)

### ![Number](Type-Number.png "Number") = isinf(![Number](Type-Number.png "Number") Value)

Returns 1 if given value is a positive infinity or -1 if given value is a negative infinity; otherwise 0. (2 ops)

### ![Number](Type-Number.png "Number") = isnan(![Number](Type-Number.png "Number") Value)

Returns 1 if given value is not a number (NaN); otherwise 0. (2 ops)

### ![Number](Type-Number.png "Number") = abs(![Number](Type-Number.png "Number") Value)

Returns the Magnitude of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = ceil(![Number](Type-Number.png "Number") Rv1)

Rounds the Argument up to the nearest Integer (2 ops)

### ![Number](Type-Number.png "Number") = ceil(![Number](Type-Number.png "Number") Value, ![Number](Type-Number.png "Number") Decimals)

Rounds Argument 1 up to Argument 2's decimal precision (2 ops)

### ![Number](Type-Number.png "Number") = floor(![Number](Type-Number.png "Number") Rv1)

Rounds the Argument down to the nearest Integer (2 ops)

### ![Number](Type-Number.png "Number") = floor(![Number](Type-Number.png "Number") Value, ![Number](Type-Number.png "Number") Decimals)

Rounds Argument 1 down to Argument 2's decimal precision (2 ops)

### ![Number](Type-Number.png "Number") = round(![Number](Type-Number.png "Number") Rv1)

Rounds the Argument to the nearest Integer (2 ops)

### ![Number](Type-Number.png "Number") = round(![Number](Type-Number.png "Number") Value, ![Number](Type-Number.png "Number") Decimals)

Rounds Argument 1 to Argument 2's decimal precision (2 ops)

### ![Number](Type-Number.png "Number") = int(![Number](Type-Number.png "Number") Rv1)

Returns the Integer part of the Argument (always rounds towards zero) (2 ops)

### ![Number](Type-Number.png "Number") = frac(![Number](Type-Number.png "Number") Rv1)

Returns the Fractional part (decimal places) of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = mod(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Modulo, returns the Remainder after Argument 1 has been divided by Argument 2. Note "mod(-1, 3) = -1" (2 ops)

### ![Number](Type-Number.png "Number") = wrap(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Performs (n1 + n2) % (n2 * 2) - n2 (2 ops)

### ![Number](Type-Number.png "Number") = clamp(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

If Arg1 = Arg3 (max) returns Arg3; otherwise returns Arg1 (2 ops)

### ![Number](Type-Number.png "Number") = inrange(![Number](Type-Number.png "Number") Value, ![Number](Type-Number.png "Number") Min, ![Number](Type-Number.png "Number") Max)

Returns 1 if N is in the interval [N2; N3], 0 otherwise. This means it is equivalent to ((N2 <= N) & (N <= N3)) (2 ops)

### ![Number](Type-Number.png "Number") = sign(![Number](Type-Number.png "Number"))

Returns the sign of argument (-1,0,1) [sign(N) = N / abs(N) ] (2 ops)

### ![Number](Type-Number.png "Number") = random()

Returns a random floating-point number between 0 and 1 [0 <= x < 1 ] (2 ops)

### ![Number](Type-Number.png "Number") = random(![Number](Type-Number.png "Number"))

Returns a random floating-point number between 0 and the specified value [0 <= x < a ] (2 ops)

### ![Number](Type-Number.png "Number") = random(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns a random floating-point number between the specified interval [a <= x < b ] (2 ops)

### ![Number](Type-Number.png "Number") = randint(![Number](Type-Number.png "Number"))

Returns a random integer from 1 to the specified value [1 <= x <= a ] (2 ops)

### ![Number](Type-Number.png "Number") = randint(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns a random integer in the specified interval [a <= x <= b ] (2 ops)

### ![Number](Type-Number.png "Number") = sqrt(![Number](Type-Number.png "Number"))

Returns the Square Root of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = cbrt(![Number](Type-Number.png "Number"))

Returns the Cube Root of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = root(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the Nth Root of the first Argument (2 ops)

### ![Number](Type-Number.png "Number") = e()

Returns Euler's Constant (2 ops)

### ![Number](Type-Number.png "Number") = exp(![Number](Type-Number.png "Number"))

Returns e to the power of the Argument (same as e()^N but shorter and faster this way) (2 ops)

### ![Vector2](Type-Vector2.png "Vector2") = frexp(![Number](Type-Number.png "Number") X)

Returns the mantissa and exponent of the given floating-point number as a vector2 (X component holds a mantissa, and Y component holds an exponent) (2 ops)

### ![Number](Type-Number.png "Number") = ln(![Number](Type-Number.png "Number"))

Returns the logarithm to base e of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = log2(![Number](Type-Number.png "Number"))

Returns the logarithm to base 2 of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = log10(![Number](Type-Number.png "Number"))

Returns the logarithm to base 10 of the Argument (2 ops)

### ![Number](Type-Number.png "Number") = log(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the logarithm to base Argument 2 of Argument 1 (2 ops)

### ![Number](Type-Number.png "Number") = inf()

Returns a huge constant (infinity) (2 ops)

### ![Number](Type-Number.png "Number") = pi()

Returns the constant PI (2 ops)

### ![Number](Type-Number.png "Number") = toRad(![Number](Type-Number.png "Number"))

Converts Degree angles to Radian angles (2 ops)

### ![Number](Type-Number.png "Number") = toDeg(![Number](Type-Number.png "Number"))

Converts Radian angles to Degree angles (2 ops)

### ![Number](Type-Number.png "Number") = acos(![Number](Type-Number.png "Number"))

Returns the inverse cosine of the argument, in degrees (2 ops)

### ![Number](Type-Number.png "Number") = asin(![Number](Type-Number.png "Number"))

Returns the inverse sine of the argument, in degrees (2 ops)

### ![Number](Type-Number.png "Number") = atan(![Number](Type-Number.png "Number"))

Returns the inverse tangent of the argument, in degrees (2 ops)

### ![Number](Type-Number.png "Number") = atan(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the inverse tangent of the arguments (arg1 / arg2), in degrees. This function accounts for positive/negative arguments, and arguments at or close to 0 (2 ops)

### ![Number](Type-Number.png "Number") = cos(![Number](Type-Number.png "Number"))

Returns the cosine of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = sec(![Number](Type-Number.png "Number"))

Returns the secant of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = sin(![Number](Type-Number.png "Number"))

Returns the sine of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = csc(![Number](Type-Number.png "Number"))

Returns the cosecant of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = tan(![Number](Type-Number.png "Number"))

Returns the tangent of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = cot(![Number](Type-Number.png "Number"))

Returns the cotangent of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = cosh(![Number](Type-Number.png "Number"))

Returns the hyperbolic cosine of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = sech(![Number](Type-Number.png "Number"))

Returns the hyperbolic secant of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = sinh(![Number](Type-Number.png "Number"))

Returns the hyperbolic sine of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = csch(![Number](Type-Number.png "Number"))

Returns the hyperbolic cosecant of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = tanh(![Number](Type-Number.png "Number"))

Returns the hyperbolic tangent of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = coth(![Number](Type-Number.png "Number"))

Returns the hyperbolic cotangent of N degrees (2 ops)

### ![Number](Type-Number.png "Number") = acosr(![Number](Type-Number.png "Number"))

Returns the inverse cosine of the argument, in radians (2 ops)

### ![Number](Type-Number.png "Number") = asinr(![Number](Type-Number.png "Number"))

Returns the inverse sine of the argument, in radians (2 ops)

### ![Number](Type-Number.png "Number") = atanr(![Number](Type-Number.png "Number"))

Returns the inverse tangent of the argument, in radians (2 ops)

### ![Number](Type-Number.png "Number") = atanr(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns the inverse tangent of the arguments (arg1 / arg2), in radians. This function accounts for positive/negative arguments, and arguments at or close to 0 (2 ops)

### ![Number](Type-Number.png "Number") = cosr(![Number](Type-Number.png "Number"))

Returns the cosine of N radians (2 ops)

### ![Number](Type-Number.png "Number") = secr(![Number](Type-Number.png "Number"))

Returns the secant of N radians (2 ops)

### ![Number](Type-Number.png "Number") = sinr(![Number](Type-Number.png "Number"))

Returns the sine of N radians (2 ops)

### ![Number](Type-Number.png "Number") = cscr(![Number](Type-Number.png "Number"))

Returns the cosecant of N radians (2 ops)

### ![Number](Type-Number.png "Number") = tanr(![Number](Type-Number.png "Number"))

Returns the tangent of N radians (2 ops)

### ![Number](Type-Number.png "Number") = cotr(![Number](Type-Number.png "Number"))

Returns the cotangent of N radians (2 ops)

### ![Number](Type-Number.png "Number") = coshr(![Number](Type-Number.png "Number"))

Returns the hyperbolic cosine of N radians (2 ops)

### ![Number](Type-Number.png "Number") = sechr(![Number](Type-Number.png "Number"))

Returns the hyperbolic secant of N radians (2 ops)

### ![Number](Type-Number.png "Number") = sinhr(![Number](Type-Number.png "Number"))

Returns the hyperbolic sine of N radians (2 ops)

### ![Number](Type-Number.png "Number") = cschr(![Number](Type-Number.png "Number"))

Returns the hyperbolic cosecant of N radians (2 ops)

### ![Number](Type-Number.png "Number") = tanhr(![Number](Type-Number.png "Number"))

Returns the hyperbolic tangent of N radians (2 ops)

### ![Number](Type-Number.png "Number") = cothr(![Number](Type-Number.png "Number"))

Returns the hyperbolic cotangent of N radians (2 ops)

### ![String](Type-String.png "String") = toString(![Number](Type-Number.png "Number") Number)

Formats a number as a string. (Numbers may be concatenated into a string without using this function) (15 ops)

### ![String](Type-String.png "String") = ![Number](Type-Number.png "Number"):toString()

Formats a number as a string. (Numbers may be concatenated into a string without using this function) (15 ops)

### ![String](Type-String.png "String") = toString(![Number](Type-Number.png "Number") Number, ![Number](Type-Number.png "Number") Base)

Formats a number as a string, using argument 2 as the base. i.e. using 16 for base would convert the number to hex (25 ops)

### ![String](Type-String.png "String") = ![Number](Type-Number.png "Number"):toString(![Number](Type-Number.png "Number") Base)

Formats a number as a string, using argument 2 as the base. i.e. using 16 for base would convert the number to hex (25 ops)