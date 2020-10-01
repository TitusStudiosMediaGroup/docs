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

# String

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):toNumber()

Parses a number from a string (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):toNumber(![Number](Type-Number.png "Number") Base)

Parses a number from a string. The argument given is the base. I.e. toNumber(16) will parse hex (20 ops)

### ![String](Type-String.png "String") = toChar(![Number](Type-Number.png "Number"))

Returns a one-character string from it's ASCII code, where 32 = argument 1 = 255. An empty string is returned for numbers outside that range (20 ops)

### ![Number](Type-Number.png "Number") = toByte(![String](Type-String.png "String"))

Returns the ASCII code of the 1st character in the string (20 ops)

### ![Number](Type-Number.png "Number") = toByte(![String](Type-String.png "String"), ![Number](Type-Number.png "Number"))

Returns the ASCII code of the Nth character in the string (20 ops)

### ![String](Type-String.png "String") = toUnicodeChar(![Number](Type-Number.png "Number"))

Returns a one-character string from it's UNICODE code (20 ops)

### ![Number](Type-Number.png "Number") = toUnicodeByte(![String](Type-String.png "String"))

Returns the Unicode code of the 1st character in the string (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):index(![Number](Type-Number.png "Number"))

Returns Nth letter of the string, formatted as a string (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):left(![Number](Type-Number.png "Number"))

Returns N amount of characters starting from the leftmost character (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):right(![Number](Type-Number.png "Number"))

Returns N amount of characters starting from the rightmost character (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):sub(![Number](Type-Number.png "Number"), ![Number](Type-Number.png "Number"))

Returns a substring, starting at the first number argument and ending at the second (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):sub(![Number](Type-Number.png "Number") Start)

Returns a substring, starting at the number argument and ending at the end of the string (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):upper()

All characters are made uppercase (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):lower()

All characters are made lowercase (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):length()

Returns the length of the string (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):unicodeLength()

Returns the unicode length of the string (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):repeat(![Number](Type-Number.png "Number"))

Repeats the input string N times (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):trim()

Trims away spaces at the beginning and end of a string (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):trimLeft()

Trims away opening spaces on the string (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):trimRight()

Trims away spaces at the end of a string (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):findRE(![String](Type-String.png "String") Pattern)

Returns the 1st occurrence of the string S using REGEX functions, returns 0 if not found (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):findRE(![String](Type-String.png "String") Pattern, ![Number](Type-Number.png "Number") Start)

Returns the 1st occurrence of the string S starting at N and going to the end of the string using REGEX functions, returns 0 if not found (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):find(![String](Type-String.png "String") Needle)

Returns the 1st occurrence of the string S, returns 0 if not found (20 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):find(![String](Type-String.png "String") Needle, ![Number](Type-Number.png "Number") Start)

Returns the 1st occurrence of the string S starting at N and going to the end of the string, returns 0 if not found (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):replace(![String](Type-String.png "String") Needle, ![String](Type-String.png "String") New)

Finds and replaces every occurrence of the first argument with the second argument (20 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):replaceRE(![String](Type-String.png "String") Pattern, ![String](Type-String.png "String") New)

Finds and replaces every occurrence of the first argument using REGEX with the second argument (20 ops)

### ![Array](Type-Array.png "Array") = ![String](Type-String.png "String"):explode(![String](Type-String.png "String") Delim)

Splits the string into an array, along the boundaries formed by the string S. See also String.Explode (5 ops)

### ![Array](Type-Array.png "Array") = ![String](Type-String.png "String"):explodeRE(![String](Type-String.png "String") Delim)

Splits the string into an array, along the boundaries formed by the string pattern S. See also String.Explode (5 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):reverse()

Returns a reversed version of S (10 ops)

### ![String](Type-String.png "String") = format(![String](Type-String.png "String") Fmt, ...)

Formats a values exactly like Lua's [http://www.lua.org/manual/5.1/manual.html#pdf-string.format string.format]. Any number and type of parameter can be passed through the "...". Prints errors to the chat area (10 ops)

### ![Array](Type-Array.png "Array") = ![String](Type-String.png "String"):match(![String](Type-String.png "String") Pattern)

runs string.match(S, S2) and returns the sub-captures as an array (10 ops)

### ![Array](Type-Array.png "Array") = ![String](Type-String.png "String"):match(![String](Type-String.png "String") Pattern, ![Number](Type-Number.png "Number") Position)

runs string.match(S, S2, N) and returns the sub-captures as an array (10 ops)

### ![Table](Type-Table.png "Table") = ![String](Type-String.png "String"):gmatch(![String](Type-String.png "String") Pattern)

runs string.gmatch(S, S2) and returns the captures in arrays in a table (10 ops)

### ![Table](Type-Table.png "Table") = ![String](Type-String.png "String"):gmatch(![String](Type-String.png "String") Pattern, ![Number](Type-Number.png "Number") Position)

runs string.gmatch(S, S2, N) and returns the captures in arrays in a table (10 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):matchFirst(![String](Type-String.png "String") Pattern)

runs string.match(S, S2) and returns the first match or an empty string if the match failed (10 ops)

### ![String](Type-String.png "String") = ![String](Type-String.png "String"):matchFirst(![String](Type-String.png "String") Pattern, ![Number](Type-Number.png "Number") Position)

runs string.match(S, S2, N) and returns the first match or an empty string if the match failed (10 ops)

### ![String](Type-String.png "String") = toUnicodeChar(...)

Returns the UTF-8 string from the given Unicode code-points (1 ops)

### ![String](Type-String.png "String") = toUnicodeChar(![Array](Type-Array.png "Array") Args)

Returns the UTF-8 string from the given Unicode code-points (1 ops)

### ![Array](Type-Array.png "Array") = ![String](Type-String.png "String"):toUnicodeByte(![Number](Type-Number.png "Number") Startpos, ![Number](Type-Number.png "Number") Endpos)

Returns the Unicode code-points from the given UTF-8 string (1 ops)

### ![Number](Type-Number.png "Number") = ![String](Type-String.png "String"):unicodeLength(![Number](Type-Number.png "Number") Startpos, ![Number](Type-Number.png "Number") Endpos)

Returns the length of the given UTF-8 string (1 ops)