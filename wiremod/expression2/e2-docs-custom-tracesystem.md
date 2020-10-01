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

# Custom/tracesystem

### ![Vector](Type-Vector.png "Vector") = rayPlaneIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Normal)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayFaceIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Normal, ![Vector](Type-Vector.png "Vector") Size, ![Number](Type-Number.png "Number") Ang)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayPolygonIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Vertex1, ![Vector](Type-Vector.png "Vector") Vertex2, ![Vector](Type-Vector.png "Vector") Vertex3)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayAABBoxIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Size)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayOBBoxIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Size, ![Angle](Type-Angle.png "Angle") Ang)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayCircleIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Normal, ![Number](Type-Number.png "Number") Radius)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = raySphereIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Number](Type-Number.png "Number") Radius)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayAAEllipsoidIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Size)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = rayOEllipsoidIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Size, ![Angle](Type-Angle.png "Angle") Ang)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = coneSphereIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Vector](Type-Vector.png "Vector") Pos, ![Number](Type-Number.png "Number") Radius, ![Number](Type-Number.png "Number") Ang)

 (0 ops)

### ![Number](Type-Number.png "Number") = tsShapeCanCreate()

 (0 ops)

### tsShapeShare(![Number](Type-Number.png "Number") Share)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeCreate(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Model, ![Number](Type-Number.png "Number") Radius, ![Number](Type-Number.png "Number") Rotation, ![Vector](Type-Vector.png "Vector") Pos, ![Vector](Type-Vector.png "Vector") Normal, ![Vector](Type-Vector.png "Vector") Size, ![Angle](Type-Angle.png "Angle") Ang, ![Vector](Type-Vector.png "Vector") Vertex1, ![Vector](Type-Vector.png "Vector") Vertex2, ![Vector](Type-Vector.png "Vector") Vertex3)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeCreate(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![String](Type-String.png "String") = tsShapePolygon(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Vertex1, ![Vector](Type-Vector.png "Vector") Vertex2, ![Vector](Type-Vector.png "Vector") Vertex3)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeModel(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Model)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeRadius(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Radius)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeRotation(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Rotation)

 (0 ops)

### ![String](Type-String.png "String") = tsShapePos(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Pos)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeVertices(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Vertex1, ![Vector](Type-Vector.png "Vector") Vertex2, ![Vector](Type-Vector.png "Vector") Vertex3)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeAng(![Number](Type-Number.png "Number") Index, ![Angle](Type-Angle.png "Angle") Ang)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeNormal(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Normal)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeSize(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Size)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeParent(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Parent)

 (0 ops)

### ![String](Type-String.png "String") = tsShapeRemove(![Number](Type-Number.png "Number") Index)

 (0 ops)

### tsShapeClear()

 (0 ops)

### Tracedata = tsRayPlaneIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRayFaceIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRayPolygonIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRayBoxIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRayCircleIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRaySphereIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRayEllipsoidIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsRayIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir)

 (0 ops)

### Tracedata = tsConeSphereIntersection(![Vector](Type-Vector.png "Vector") Start, ![Vector](Type-Vector.png "Vector") Dir, ![Number](Type-Number.png "Number") Angle)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:sortByDistance(![Vector](Type-Vector.png "Vector") Pos)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:count()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:hit()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:hit(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:hitAngle()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:hitAngle(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:index()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:index(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:distance()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:distance(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:radius()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:radius(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:rotation()

 (0 ops)

### ![Number](Type-Number.png "Number") = Tracedata:rotation(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![String](Type-String.png "String") = Tracedata:model()

 (0 ops)

### ![String](Type-String.png "String") = Tracedata:model(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:hitPos()

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:hitPos(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:pos()

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:pos(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:vertices()

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:vertices(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Angle](Type-Angle.png "Angle") = Tracedata:ang()

 (0 ops)

### ![Angle](Type-Angle.png "Angle") = Tracedata:ang(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:hitNormal()

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:hitNormal(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:size()

 (0 ops)

### ![Vector](Type-Vector.png "Vector") = Tracedata:size(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Entity](Type-Entity.png "Entity") = Tracedata:parent()

 (0 ops)

### ![Entity](Type-Entity.png "Entity") = Tracedata:parent(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Entity](Type-Entity.png "Entity") = Tracedata:entity()

 (0 ops)

### ![Entity](Type-Entity.png "Entity") = Tracedata:entity(![Number](Type-Number.png "Number") Index)

 (0 ops)

### ![Entity](Type-Entity.png "Entity") = Tracedata:owner()

 (0 ops)

### ![Entity](Type-Entity.png "Entity") = Tracedata:owner(![Number](Type-Number.png "Number") Index)

 (0 ops)