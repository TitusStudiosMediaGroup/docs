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
* [custom/trackasmlib_wire](e2-docs-custom-trackasmlib_wire)
* [custom/wiring](e2-docs-custom-wiring)
***

# Custom/trackasmlib_wire

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):trackasmlibGenActivePointINS(![Entity](Type-Entity.png "Entity") Ucsent, ![String](Type-String.png "String") Stype, ![String](Type-String.png "String") Sname, ![Number](Type-Number.png "Number") Npoint)

 (50 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):trackasmlibGenActivePointDSV(![Entity](Type-Entity.png "Entity") Ucsent, ![String](Type-String.png "String") Stype, ![String](Type-String.png "String") Sname, ![Number](Type-Number.png "Number") Npoint)

 (50 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):trackasmlibSnapEntity(![Vector](Type-Vector.png "Vector") Trhitpos, ![String](Type-String.png "String") Hdmodel, ![Number](Type-Number.png "Number") Hdpoid, ![Number](Type-Number.png "Number") Nactradius, ![Number](Type-Number.png "Number") Enflatten, ![Number](Type-Number.png "Number") Enigntyp, ![Vector](Type-Vector.png "Vector") Ucsoffpos)

 (100 ops)

### ![Array](Type-Array.png "Array") = trackasmlibSnapNormal(![Vector](Type-Vector.png "Vector") Ucspos, ![Angle](Type-Angle.png "Angle") Ucsang, ![String](Type-String.png "String") Hdmodel, ![Number](Type-Number.png "Number") Hdpoid, ![Vector](Type-Vector.png "Vector") Ucsoffpos)

 (80 ops)

### ![Number](Type-Number.png "Number") = trackasmlibIsPiece(![String](Type-String.png "String") Smodel)

 (30 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):trackasmlibIsPiece()

 (30 ops)

### ![Array](Type-Array.png "Array") = trackasmlibGetOffset(![String](Type-String.png "String") Smodel, ![Number](Type-Number.png "Number") Nid)

 (80 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetOffset(![Number](Type-Number.png "Number") Nid)

 (80 ops)

### ![String](Type-String.png "String") = trackasmlibGetType(![String](Type-String.png "String") Smodel)

 (30 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetType()

 (30 ops)

### ![String](Type-String.png "String") = trackasmlibGetName(![String](Type-String.png "String") Smodel)

 (30 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetName()

 (30 ops)

### ![Number](Type-Number.png "Number") = trackasmlibGetPointsCount(![String](Type-String.png "String") Smodel)

 (30 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetPointsCount()

 (30 ops)

### ![Number](Type-Number.png "Number") = trackasmlibHasAdditions(![String](Type-String.png "String") Smodel)

 (30 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):trackasmlibHasAdditions()

 (30 ops)

### ![Number](Type-Number.png "Number") = trackasmlibGetAdditionsCount(![String](Type-String.png "String") Smodel)

 (50 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetAdditionsCount()

 (50 ops)

### ![Array](Type-Array.png "Array") = trackasmlibGetAdditionsLine(![String](Type-String.png "String") Smodel)

 (60 ops)

### ![Array](Type-Array.png "Array") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetAdditionsLine(![Number](Type-Number.png "Number") Nid)

 (60 ops)

### ![Array](Type-Array.png "Array") = trackasmlibGetProperty(![String](Type-String.png "String") Stype)

 (15 ops)

### ![Array](Type-Array.png "Array") = trackasmlibGetProperty()

 (15 ops)

### ![Entity](Type-Entity.png "Entity") = trackasmlibMakePiece(![String](Type-String.png "String") Smodel, ![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang, ![Number](Type-Number.png "Number") Nmass, ![String](Type-String.png "String") Sbgpid, ![Number](Type-Number.png "Number") Nr, ![Number](Type-Number.png "Number") Ng, ![Number](Type-Number.png "Number") Nb)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibMakePiece(![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang, ![Number](Type-Number.png "Number") Nmass, ![String](Type-String.png "String") Sbgpid, ![Number](Type-Number.png "Number") Nr, ![Number](Type-Number.png "Number") Ng, ![Number](Type-Number.png "Number") Nb)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = trackasmlibMakePiece(![String](Type-String.png "String") Smodel, ![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang, ![Number](Type-Number.png "Number") Nmass, ![String](Type-String.png "String") Sbgpid)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibMakePiece(![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang, ![Number](Type-Number.png "Number") Nmass, ![String](Type-String.png "String") Sbgpid)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = trackasmlibMakePiece(![String](Type-String.png "String") Smodel, ![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang, ![Number](Type-Number.png "Number") Nmass)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibMakePiece(![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang, ![Number](Type-Number.png "Number") Nmass)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = trackasmlibMakePiece(![String](Type-String.png "String") Smodel, ![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibMakePiece(![Vector](Type-Vector.png "Vector") Vpos, ![Angle](Type-Angle.png "Angle") Aang)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibMakePiece(![Vector](Type-Vector.png "Vector") Vpos)

 (50 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibApplyPhysicalAnchor(![Entity](Type-Entity.png "Entity") Ebase, ![Number](Type-Number.png "Number") Nwe, ![Number](Type-Number.png "Number") Nnc, ![Number](Type-Number.png "Number") Nnw)

 (15 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):trackasmlibApplyPhysicalSettings(![Number](Type-Number.png "Number") Npi, ![Number](Type-Number.png "Number") Nfr, ![Number](Type-Number.png "Number") Ngr)

 (15 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):trackasmlibAttachAdditions()

 (35 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):trackasmlibAttachBodyGroups(![String](Type-String.png "String") Sbgpid)

 (20 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetBodyGroups()

 (20 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):trackasmlibGetSkin()

 (20 ops)