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

# Files

### fileLoad(![String](Type-String.png "String") Filename)

Loads specified file to the server (20 ops)

### ![Number](Type-Number.png "Number") = fileCanLoad()

Returns 1 if the file can be loaded (5 ops)

### ![Number](Type-Number.png "Number") = fileLoaded()

Returns whether or not the file has been loaded onto the server (5 ops)

### ![Number](Type-Number.png "Number") = fileLoading()

Returns whether a file is currently uploading (5 ops)

### ![Number](Type-Number.png "Number") = fileStatus()

Returns the status of the upload in progress. Returns one of _FILE_UNKNOWN, _FILE_OK, _FILE_TIMEOUT, _FILE_404 or _FILE_TRANSFER_ERROR (5 ops)

### ![String](Type-String.png "String") = fileName()

Returns the name of the last uploaded file, or an empty string if there is no currently uploaded file (5 ops)

### ![String](Type-String.png "String") = fileRead()

Returns the contents of the last uploaded file, or an empty string if there is no currently uploaded file (10 ops)

### ![Number](Type-Number.png "Number") = fileMaxSize()

Returns the maximum file size that can be uploaded or downloaded. Default is 300 KiB (5 ops)

### ![Number](Type-Number.png "Number") = fileCanWrite()

Returns 1 if the file can be written (5 ops)

### fileWrite(![String](Type-String.png "String") Filename, ![String](Type-String.png "String") Data)

Writes string data to the file overwriting it (20 ops)

### fileAppend(![String](Type-String.png "String") Filename, ![String](Type-String.png "String") Data)

Adds string data to the end of the file (20 ops)

### fileList(![String](Type-String.png "String") Dir)

Returns an array of file names that have been loaded (20 ops)

### ![Number](Type-Number.png "Number") = fileCanList()

Returns 1 if the file list can be uploaded to the server (5 ops)

### ![Number](Type-Number.png "Number") = fileLoadedList()

If the list has been loaded and it is called, it will return 1. Any time after that until a new list is loaded it will return 0 (5 ops)

### ![Number](Type-Number.png "Number") = fileLoadingList()

Returns whether a list is currently uploading (5 ops)

### ![Array](Type-Array.png "Array") = fileReadList()

Returns the contents of the last uploaded list (5 ops)

### runOnFile(![Number](Type-Number.png "Number") Active)

Specifies whether the E2 will run when a file finishes uploading (5 ops)

### ![Number](Type-Number.png "Number") = fileClk()

Returns whether the execution was run because a file finished uploading (5 ops)

### ![Number](Type-Number.png "Number") = fileClk(![String](Type-String.png "String") Filename)

Returns whether the execution was run because a file finished uploading and was that file of a specific file name (5 ops)

### runOnList(![Number](Type-Number.png "Number") Active)

Specifies whether the E2 will run when a list finishes uploading (5 ops)

### ![Number](Type-Number.png "Number") = fileListClk()

Returns whether the execution was run because a list was uploaded to the server (5 ops)

### ![Number](Type-Number.png "Number") = fileListClk(![String](Type-String.png "String") Dir)

Returns whether the execution was run because a list with specified name was uploaded to the server (5 ops)