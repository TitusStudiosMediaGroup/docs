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

# Npc

### ![Entity](Type-Entity.png "Entity"):npcGoWalk(![Vector](Type-Vector.png "Vector") Rv2)

Tells the NPC to walk to position V (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcGoRun(![Vector](Type-Vector.png "Vector") Rv2)

Tells the NPC to run to position V (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcAttack()

Tells the NPC to use their melee attack (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcShoot()

Tells the NPC to shoot their gun (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcFace(![Vector](Type-Vector.png "Vector") Rv2)

This will rotate the NPC to face position V. This is purely aesthetic and can't be used to aim their weapon (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcGiveWeapon()

Gives the NPC an SMG (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcGiveWeapon(![String](Type-String.png "String") Rv2)

Gives the NPC a weapon. Example: E:npcGiveWeapon("pistol"). Other arguments include "ar2", "crowbar", "357", "shotgun", "crossbow", "rpg", "frag", etc. Other such as the bugbait or slam may be buggy (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcStop()

Stops any anything the NPC is doing, including things it decided to do by itself (5 ops)

### ![Entity](Type-Entity.png "Entity") = ![Entity](Type-Entity.png "Entity"):npcGetTarget()

Returns what the npc is currently targeting (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcSetTarget(![Entity](Type-Entity.png "Entity") Ent)

Sets the npcs current target (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcRelationship(![Entity](Type-Entity.png "Entity") Rv2, ![String](Type-String.png "String") Rv3, ![Number](Type-Number.png "Number") Rv4)

Will set the NPC's relationship to the specified entity to the S input, priority N. Priority is any number between 0 and 999. The relationship string can be either "like", "neutral", "hate" or "fear". Same goes for all other relationship functions (5 ops)

### ![Entity](Type-Entity.png "Entity"):npcRelationship(![String](Type-String.png "String") Rv2, ![String](Type-String.png "String") Rv3, ![Number](Type-Number.png "Number") Rv4)

Same as E:npcRelationship(entity,string,number), but sets relationship to an entire class specified by the first string. Example: "npc_manhack", "prop_physics" (5 ops)

### ![Number](Type-Number.png "Number") = ![Entity](Type-Entity.png "Entity"):npcRelationshipByOwner(![Entity](Type-Entity.png "Entity") Rv2, ![String](Type-String.png "String") Rv3, ![Number](Type-Number.png "Number") Rv4)

Sets the NPC's relationship to all currently existing NPCs owned by player E. Returns number of entities added to relationships (5 ops)

### ![String](Type-String.png "String") = ![Entity](Type-Entity.png "Entity"):npcDisp(![Entity](Type-Entity.png "Entity") Rv2)

Returns the NPC's relationship to entity E (5 ops)