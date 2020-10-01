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

# Timer

### interval(![Number](Type-Number.png "Number") Rv1)

Sets a one-time timer with name "interval" and delay in milliseconds (minimum delay for timers is 10ms) (20 ops)

### timer(![String](Type-String.png "String") Rv1, ![Number](Type-Number.png "Number") Rv2)

Sets a one-time timer with entered name and delay in milliseconds (20 ops)

### stoptimer(![String](Type-String.png "String") Rv1)

Stops a timer, can stop interval with stoptimer("interval") (5 ops)

### ![Number](Type-Number.png "Number") = clk()

Returns 1 if the current execution was caused by the interval (1 ops)

### ![Number](Type-Number.png "Number") = clk(![String](Type-String.png "String") Rv1)

Returns 1 if the current execution was caused by the inserted name (1 ops)

### ![String](Type-String.png "String") = clkName()

Returns the name of the timer that caused current execution (1 ops)

### ![Array](Type-Array.png "Array") = getTimers()

Returns an array of all timers used in the E2 (1 ops)

### stopAllTimers()

Stops all timers (1 ops)

### ![Number](Type-Number.png "Number") = curtime()

Returns the current game time since server-start in seconds (1 ops)

### ![Number](Type-Number.png "Number") = realtime()

Returns the current real time since server-start in seconds (1 ops)

### ![Number](Type-Number.png "Number") = systime()

Returns a highly accurate time (also in seconds) since the server was started. Ideal for benchmarking (1 ops)

### ![Table](Type-Table.png "Table") = date()

Returns the server's current time and date (10 ops)

### ![Table](Type-Table.png "Table") = date(![Number](Type-Number.png "Number") Time)

Returns the specified unix time (10 ops)

### ![Table](Type-Table.png "Table") = dateUTC()

Returns the server's current time and date in UTC (10 ops)

### ![Table](Type-Table.png "Table") = dateUTC(![Number](Type-Number.png "Number") Time)

Returns the specified unix time in UTC (10 ops)

### ![Number](Type-Number.png "Number") = time(![String](Type-String.png "String") Component)

Returns numerical time/date info from the server. Possible arguments: "year", "month", "day", "hour", "min", "sec", "wday" (weekday, Sunday is 1), "yday" (day of the year), and "isdst" (daylight saving flag 0/1) (10 ops)

### ![Number](Type-Number.png "Number") = time()

Returns the time in seconds (2 ops)

### ![Number](Type-Number.png "Number") = time(![Table](Type-Table.png "Table") Data)

Attempts to construct the time from the data in the given table (same as lua's os.time). The table structure must be the same as in the date() functions. If any values are missing or of the wrong type, that value is ignored (it will be nil) (2 ops)