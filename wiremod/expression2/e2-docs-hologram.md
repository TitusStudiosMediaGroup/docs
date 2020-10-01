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

# Hologram

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position, ![Vector](Type-Vector.png "Vector") Scale, ![Angle](Type-Angle.png "Angle") Ang, ![Vector](Type-Vector.png "Vector") Color, ![String](Type-String.png "String") Model)

Index, Position, Scale, Angle, Color (RGB), Model
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position, ![Vector](Type-Vector.png "Vector") Scale, ![Angle](Type-Angle.png "Angle") Ang, ![Vector4](Type-Vector4.png "Vector4") Color, ![String](Type-String.png "String") Model)

Index, Position, Scale, Angle, Color (RGBA), Model
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position, ![Vector](Type-Vector.png "Vector") Scale, ![Angle](Type-Angle.png "Angle") Ang, ![Vector](Type-Vector.png "Vector") Color)

Index, Position, Scale, Angle, Color (RGB)
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position, ![Vector](Type-Vector.png "Vector") Scale, ![Angle](Type-Angle.png "Angle") Ang, ![Vector4](Type-Vector4.png "Vector4") Color)

Index, Position, Scale, Angle, Color (RGBA)
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position, ![Vector](Type-Vector.png "Vector") Scale, ![Angle](Type-Angle.png "Angle") Ang)

Index, Position, Scale, Angle
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position, ![Vector](Type-Vector.png "Vector") Scale)

Index, Position, Scale
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position)

Index, Position
Creates a new hologram entity (30 ops)

### ![Entity](Type-Entity.png "Entity") = holoCreate(![Number](Type-Number.png "Number") Index)

Index
Creates a new hologram entity (30 ops)

### holoDelete(![Number](Type-Number.png "Number") Index)

Removes a hologram (20 ops)

### holoDeleteAll()

Removes all holograms made by this E2 (20 ops)

### holoDeleteAll(![Number](Type-Number.png "Number") All)

 (20 ops)

### holoReset(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Model, ![Vector](Type-Vector.png "Vector") Scale, ![Vector](Type-Vector.png "Vector") Color, ![String](Type-String.png "String") Material)

Similar to holoCreate, but reusing the old entity (20 ops)

### ![Number](Type-Number.png "Number") = holoCanCreate()

Returns 1 when holoCreate() will successfully create a new hologram until the Max limit is reached
Replaces holoRemainingSpawns() (2 ops)

### ![Number](Type-Number.png "Number") = holoRemainingSpawns()

Returns how many holograms can be created this execution (2 ops)

### ![Number](Type-Number.png "Number") = holoAmount()

 (2 ops)

### ![Number](Type-Number.png "Number") = holoMaxAmount()

 (2 ops)

### holoScale(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Scale)

Sets the scale of the given hologram, as a multiplier (15 ops)

### ![Vector](Type-Vector.png "Vector") = holoScale(![Number](Type-Number.png "Number") Index)

Returns the scale of the given hologram (15 ops)

### holoScaleUnits(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Size)

Sets the scale of the given hologram, in source units (15 ops)

### ![Vector](Type-Vector.png "Vector") = holoScaleUnits(![Number](Type-Number.png "Number") Index)

Returns the scale of the given hologram in source units (15 ops)

### holoBoneScale(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Boneindex, ![Vector](Type-Vector.png "Vector") Scale)

Sets the scale of the given hologram bone, as a multiplier (15 ops)

### holoBoneScale(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Bone, ![Vector](Type-Vector.png "Vector") Scale)

Sets the scale of the given hologram named bone, as a multiplier (15 ops)

### ![Vector](Type-Vector.png "Vector") = holoBoneScale(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Boneindex)

Returns the scale of the given hologram bone (15 ops)

### ![Vector](Type-Vector.png "Vector") = holoBoneScale(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Bone)

Returns the scale of the given hologram named bone (15 ops)

### ![Number](Type-Number.png "Number") = holoClipsAvailable()

Returns the maximum number of clipping planes allowed per hologram (1 ops)

### holoClipEnabled(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Enabled)

Enables / disables clipping for a hologram with specified index (15 ops)

### holoClipEnabled(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Clipidx, ![Number](Type-Number.png "Number") Enabled)

Enables / disables clipping for a hologram with specified index. Clip index is for use with multiple clipping planes (15 ops)

### holoClip(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Origin, ![Vector](Type-Vector.png "Vector") Normal, ![Number](Type-Number.png "Number") Isglobal)

Defines a plane used to clip a hologram specified by it's position, direction and number 1/0 whether the position should be global or local to the hologram (15 ops)

### holoClip(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Clipidx, ![Vector](Type-Vector.png "Vector") Origin, ![Vector](Type-Vector.png "Vector") Normal, ![Number](Type-Number.png "Number") Isglobal)

Defines a plane used to clip a hologram specified by it's index, position, direction and number 1/0 whether the position should be global or local to the hologram (15 ops)

### holoClip(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Origin, ![Vector](Type-Vector.png "Vector") Normal, ![Entity](Type-Entity.png "Entity") Localent)

Defines a plane used to clip a hologram specified by it's position, and direction local to the given entity (15 ops)

### holoClip(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Clipidx, ![Vector](Type-Vector.png "Vector") Origin, ![Vector](Type-Vector.png "Vector") Normal, ![Entity](Type-Entity.png "Entity") Localent)

Defines a plane used to clip a hologram specified by it's index, position, and direction local to the given entity (15 ops)

### holoPos(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Position)

Sets the position of the hologram (15 ops)

### holoAng(![Number](Type-Number.png "Number") Index, ![Angle](Type-Angle.png "Angle") Ang)

Sets the angle of the hologram (15 ops)

### holoColor(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Color)

Sets the color of the hologram (15 ops)

### holoColor(![Number](Type-Number.png "Number") Index, ![Vector4](Type-Vector4.png "Vector4") Color)

Sets the color and alpha of the hologram (15 ops)

### holoColor(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Color, ![Number](Type-Number.png "Number") Alpha)

Sets the color and alpha of the hologram (15 ops)

### holoAlpha(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Alpha)

Sets the transparency (0-255) of the hologram (15 ops)

### holoShadow(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Has_shadow)

Enables the hologram's shadow (10 ops)

### holoDisableShading(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Disable)

If 1, supresses engine lighting when drawing this hologram (10 ops)

### ![Array](Type-Array.png "Array") = holoModelList()

Returns the list of valid models
See holoModelAny() (10 ops)

### ![Number](Type-Number.png "Number") = holoModelAny()

Returns 1 if models outside of holoModelList can be used.
Reads convar 'wire_holograms_modelany' (1 ops)

### holoModel(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Model)

Sets the model.
Must be from holoModelList unless wire_holograms_modelany is 1 (see holoModelAny()) (10 ops)

### holoModel(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Model, ![Number](Type-Number.png "Number") Skin)

Sets the model and skin.
Must be from holoModelList unless wire_holograms_modelany is 1 (see holoModelAny()) (10 ops)

### holoSkin(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Skin)

Changes the skin of a hologram (10 ops)

### holoMaterial(![Number](Type-Number.png "Number") Index, ![String](Type-String.png "String") Material)

Sets the overlay material of the hologram (10 ops)

### holoPlayerColor(![Number](Type-Number.png "Number") Index, ![Vector](Type-Vector.png "Vector") Color)

Sets the sub-color of a hologram with player model such as clothes or physgun (10 ops)

### holoRenderFX(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Effect)

Changes the RenderFX for a hologram (10 ops)

### holoBodygroup(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Bgrp_id, ![Number](Type-Number.png "Number") Bgrp_subid)

Index, Group ID, Group SubID
Sets the bodygroups of the given hologram (10 ops)

### ![Number](Type-Number.png "Number") = holoBodygroups(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Bgrp_id)

Index, Group ID
Returns the number of bodygroups in the Group ID of the given hologram (10 ops)

### holoVisible(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ply, ![Number](Type-Number.png "Number") Visible)

If 0, prevents a specific player from seeing the hologram (10 ops)

### holoVisible(![Number](Type-Number.png "Number") Index, ![Array](Type-Array.png "Array") Players, ![Number](Type-Number.png "Number") Visible)

If 0, prevents an array of players from seeing the hologram (10 ops)

### holoParent(![Number](Type-Number.png "Number") Index, ![Number](Type-Number.png "Number") Otherindex)

Parents the hologram to another hologram (40 ops)

### holoParent(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent)

Parents the hologram to an entity (40 ops)

### holoParentAttachment(![Number](Type-Number.png "Number") Index, ![Entity](Type-Entity.png "Entity") Ent, ![String](Type-String.png "String") Attachmentname)

Parents the hologram to an entity's bone by its attachment name (40 ops)

### holoUnparent(![Number](Type-Number.png "Number") Index)

Un-parents the hologram (40 ops)

### ![Entity](Type-Entity.png "Entity") = holoEntity(![Number](Type-Number.png "Number") Index)

Returns the entity corresponding to the hologram given by the specified index (2 ops)

### ![Number](Type-Number.png "Number") = holoIndex(![Entity](Type-Entity.png "Entity") Ent)

Returns the index of the given hologram entity (30 ops)