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

# Sound

### soundPlay(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path)

Plays sound from the E2 chip. soundPlay(int Index, int Duration, string Path to File) (25 ops)

### soundPlay(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path)

Plays sound from the E2 chip. soundPlay(string Index, int Duration, string Path to File) (25 ops)

### ![Entity](Type-Entity.png "Entity"):soundPlay(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path)

Plays sound from an entity. soundPlay(string Index, int Duration, string Path to File) (25 ops)

### ![Entity](Type-Entity.png "Entity"):soundPlay(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path)

Plays sound from an entity. soundPlay(int Index, int Duration, string Path to File) (25 ops)

### soundPlay(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path, ![Number](Type-Number.png "Number") Fade)

Plays sound from the E2 chip. soundPlay(int Index, int Duration, string Path to File, int FadeTime) (25 ops)

### soundPlay(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path, ![Number](Type-Number.png "Number") Fade)

Plays sound from the E2 chip. soundPlay(string Index, int Duration, string Path to File, int FadeTime) (25 ops)

### ![Entity](Type-Entity.png "Entity"):soundPlay(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path, ![Number](Type-Number.png "Number") Fade)

Plays sound from an entity. soundPlay(string Index, int Duration, string Path to File, int FadeTime) (25 ops)

### ![Entity](Type-Entity.png "Entity"):soundPlay(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Duration, ![String](Type-String.png "String") Path, ![Number](Type-Number.png "Number") Fade)

Plays sound from an entity. soundPlay(int Index, int Duration, string Path to File, int FadeTime) (25 ops)

### soundStop(![String](Type-String.png "String") Index)

Stops the sound stored at the string index and removes the entry (5 ops)

### soundStop(![Number](Type-Number.png "Number") Index)

Stops the sound stored at the integer index and removes the entry (5 ops)

### soundStop(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Fadetime)

Fades the sound stored at the string index in the integer input's amount of seconds and removes the entry (5 ops)

### soundStop(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Fadetime)

Fades the sound stored at the first input's integer index in the second input's amount of seconds and removes the entry (5 ops)

### soundVolume(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Volume)

soundVolume(string Index, Volume), where Volume is a number between 0 and 1. Default Volume is 1 (5 ops)

### soundVolume(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Volume)

soundVolume(integer Index, Volume), where Volume is a number between 0 and 1. Default Volume is 1 (5 ops)

### soundVolume(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Volume, ![Number](Type-Number.png "Number") Fadetime)

soundVolume(integer Index, Volume, FadeTime), where Volume is a number between 0 and 1. Default Volume is 1 (5 ops)

### soundVolume(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Volume, ![Number](Type-Number.png "Number") Fadetime)

soundVolume(string Index, Volume, FadeTime), where Volume is a number between 0 and 1. Default Volume is 1 (5 ops)

### soundPitch(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Pitch)

soundPitch(integer Index, integer Pitch) Default Pitch is 100, max is 255. Pitch is scaled linearly (like frequency), rather than by octave (5 ops)

### soundPitch(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Pitch)

soundPitch(string Index, integer Pitch) Default Pitch is 100, max is 255. Pitch is scaled linearly (like frequency), rather than by octave (5 ops)

### soundPitch(![String](Type-String.png "String") Index, ![Number](Type-Number.png "Number") Pitch, ![Number](Type-Number.png "Number") Fadetime)

soundPitch(string Index, integer Pitch, integer Fadetime) Default Pitch is 100, max is 255. Pitch is scaled linearly (like frequency), rather than by octave (5 ops)

### soundPitch(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Pitch, ![Number](Type-Number.png "Number") Fadetime)

soundPitch(integer Index, integer Pitch, integer Fadetime) Default Pitch is 100, max is 255. Pitch is scaled linearly (like frequency), rather than by octave (5 ops)

### soundPurge()

Clears the sound table and stops all sounds (5 ops)

### ![Number](Type-Number.png "Number") = soundDuration(![String](Type-String.png "String") Sound)

soundDuration(string Path to File) Returns the duration of the sound. Note: If the server hasn't the file it returns 60 (5 ops)