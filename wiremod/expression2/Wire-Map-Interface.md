# About
First of all let me explain what the Wire Map Interface (WMI) is.

The WMI is like bridge between the map and Wiremod, it is an entity (`info_wiremapinterface`) that is able to give other entities wire ports. E2 Wirelinks and Highspeed/Memory wire ports are NOT supported.

This point entity is made for the use in the Valve Hammer Editor and is invisible in-game. It supports all popular data types (see at the bottom), it is easy to use and it is shipped with Wiremod.

If Wiremod is not installed/loaded, the entity will be not loaded, there will be a message in the console that `info_wiremapinterface` was not found and that it will be ignored. The map will run just fine, beside that you can't use the wire ports of course.

# What you have to know
If you want to use this entity you should know this:
* How to use Wiremod.
* How to use the Input/Output system of the editor.
* How to add entities to the map and how to set them up.
* What *.fgd-files are and how to install/use them.
* How to make and compile functional maps.

I can not explain the basics, as the text would just get beyond the scope. If you don't know the above points you should learn them first and come back.
Please don't mind my German GUI (Abbrechen/Übernehmen = Cancel/Apply) in the screen shots.

# For server admins
## Prop protection and controlling
You can control the use of the WMI by disabling or enabling it using the ConVar below. If you want a per player controlling, you will have to use a prop protection addon.

## ConVars
* `sv_wire_mapinterface 1/0` - Activate or deactivate the wire map interface. Default: 1

# For mappers
## The *.fgd-file
Before you can use the WMI in the Hammer Editor you have to load the file `wiremod.fgd` in the editor. You can find it the root folder of your copy of Wiremod. If you can't find it then you can use [this](https://github.com/wiremod/wire/blob/master/wiremod.fgd). The `wiremod.fgd` requires `garrysmod.fgd`. It is found in the root folder of your Garry's Mod copy.

## The entity properties
If your editor successfully loaded the *.fgd-file and you should be able create a `info_wiremapinterface` entity easily. If you open its properties menu then you should see this:
![Entity properties](http://i.imgur.com/4gCeJH1.png)

This following table explains the key names: (\<N\> is the number).

|Property Name|Key Name|Description|Type|Default Value|
|---|---|---|---|---|
|Name|targetname|The name of the interface entity.|String (entity name)|\<none\>|
|Wire Entity|wire_entity_name|The interface gives up to 32 entities with this targetname wire ports.|String (entity name)|\<none\>|
|Minimum Trigger Time|min_trigger_time|The minimum time in seconds between two in-/output triggers. It's usefull to prevent lags.|Floating Number|0.01|
|Wire Input \<N\> Name|input\<N\>_name|The name of the Nth input.|String|\<none\>|
|Wire Input \<N\> Type|input\<N\>_type|The type of the Nth input. See data type section!|int number (choices)|0 (Normal)|
|Wire Input \<N\> Description|input\<N\>_desc|The description of the Nth input. It's shown behind the input name in-game.|String|\<none\>|
|Wire Input \<N\> Code|input\<N\>_lua|The the code when Nth inputs got triggered. See Lua section!|String|\<none\>|
|Wire Output \<N\> Name|output\<N\>_name|The name of the Nth output.|String|\<none\>|
|Wire Output \<N\> Type|output\<N\>_type|The type of the Nth output. See data type section!|int number (choices)|0 (Normal)|
|Wire Output \<N\> Description|output\<N\>_desc|The description of the Nth output. It's shown behind the output name in-game.|String|\<none\>|

## The Hammer outputs
Setting of names and types of entities and ports alone will not work. You have to also connect the interface's Hammer outputs to other entities. What Hammer inputs you connect them is your choice. In this screenshot I connected them to a door:

![Entity outputs](http://i.imgur.com/MuqBDHk.png)

Valid outputs are: (\<N\> is the number):

|Name|Description|Type|
|---|---|---|
|OnResetWireInput\<N\>|Fired when the Nth wire input got reset. Useful if you have something that isn't zero by default.|Void|
|OnWireInput\<N\>|Fired when the Nth wire input got triggered. Leave the override parameter empty, if you want to use the input value!|String|
|OnWireEntsCreated|Fires when Wire In-/Outputs entities have been created. The entity is ready to use.|Void|
|OnWireEntsRemoved|Fires when Wire In-/Outputs entities have been removed. The entity is ready to use.|Void|
|OnWireEntsReady|Fires when Wire In-/Outputs entities have been created or removed. The entity is ready to use.|Void|
|OnWireEntsStartChanging|Fires when the wire map interface entity is adding or removing Wire In-/Outputs entities. The entity can't be used yet.|Void|

## The Hammer inputs
Of course this entity has also Hammer inputs, they are useful if you want to build a wire-input-entity-dispenser or if you want to make a kind of a puzzle map for instance.

Valid inputs are: (\<N\> is the number):

|Name|Description|Type|
|---|---|---|
|TriggerWireOutput\<N\>|Sets the Nth wire output to the given var when trigged.|String|
|AddEntity|Gives the wire ports to calling entity.|Void|
|RemoveEntity|Remove the wire ports from the calling entity.|Void|
|AddEntities|Adds entities by name that will get wire ports.|String (entity name)|
|RemoveEntities|Remove the wire ports from the named entities.|String (entity name)|
|RemoveAllEntities|Remove the wire ports from all entities.|Void|
|Activate|Allow the triggering from wire inputs and the updating of wire outputs.|Void|
|Deactivate|Disallow the triggering from wire inputs and the updating of wire outputs.|Void|
|Toggle|Toggle the above status.|Void|

### Note
Keep in mind that the **adding and removing of port entities is asynchronous**, because of performance and networking reasons. While the interface is adding or removing ports entities, it can't accept orders that change the list of entities!

You have to wait till the entity Hammer output `OnWireEntsReady` got fired, before you can use it again.

## The spawnflags 
I think this screenshot should explain enough. These are for built-in entity protecting, removal behavior, wire rendering, status and for the **activating of the Lua feature**

![Entity outputs](http://i.imgur.com/TKVKg8e.png)

### The Lua feature (Advanced)
If you enter a into the `Wire Input <N> Code` or `input<N>_lua` field _AND_ you activate the `Run given Lua codes (For advanced users!)` flag then it gets ran when the Nth input got triggered. The following table shows you the globals that are available inside the code's scope:

|Variable|Description|Type|
|---|---|---|
|WIRE_NAME|The name of the input.|String|
|WIRE_VALUE|The value of the input.|\<varying\>|
|WIRE_WIRED|Is the input wired?|Boolean|
|WIRE_CALLER|The interface entity.|Entity|
|WIRE_ACTIVATOR|The entity that has the input.|Entity|

This table shows some Lua methods of the interface:

|Name|Takes|Returns|Description|
|---|---|---|---|
|Entity:AddEntitiesByName|String|\<Nothing\>|Adds entities with the given name to the list and give them wire ports.|
|Entity:AddEntitiesByTable|Table|\<Nothing\>|Adds entities in given table to the list and give them wire ports.|
|Entity:RemoveAllEntities|\<Nothing\>|\<Nothing\>|Removes the wire ports from all the interface's entities.|
|Entity:RemoveEntitiesByName|String|\<Nothing\>|Removes the wire ports from the interface's entities that has the given name.|
|Entity:RemoveEntitiesByTable|Table|\<Nothing\>|Removes the wire ports from the interface's entities that has the given table.|
|Entity:GetWiredEntities|\<Nothing\>|Table|Returns a table of all interface's wire ports entities.|
|Entity:SetWiredEntities|Table|\<Nothing\>|Removes the wire ports from all the interface's entities and then adds wire ports to all entities in the given table.|

### Note
Keep in mind that the **adding and removing of port entities is asynchronous**, because of performance and networking reasons. While the interface is adding or removing ports entities, it can't accept orders that change the list of ports entities!

If you want to check if the entity is working then you have to check if the variable `entity.WirePortsChanged` is true

### Important Note
**Warning:** Similar to the `lua_run` entity you have to be **very careful** when you put Lua code in a WMI entity. There is a **limit of 512 chars** in each field and you have to **avoid double quotation marks (")** and replace them with single quotation marks ('). There is no way around, it's a problem of the Hammer editor! **Carelessness may corrupt the map!**

## Supported data types
As said in the beginning the WMI supports all common data types. This is a table of all supported data types and how they are converted:

|ID|Wire Data Type|Lua Data Type|How it is converted to wire output?|How it is converted to wire input?|
|---|---|---|---|---|
|0|NORMAL|Number|Number from String.|Number to String.|
|1|NORMAL (Toggle)|Number (0 or 1)|Toggling between 0 and 1 each time it is triggered.|It triggers the input only when value is above 0. (Useful inputs for wired buttons.)|
|2|STRING|String|String is string|String is string
|3|VECTOR2|Table with 2 indexes|Get the first 2 numbers separated by spaces from a string.|Get the 2 values and put them separated by spaces in to a string.|
|4|VECTOR|Vector|Get the first 3 numbers separated by spaces from a string.|Get the 3 values and put them separated by spaces in to a string.|
|5|VECTOR4|Table with 4 indexes|Get the first 4 numbers separated by spaces from a string.|Get the 4 values and put them separated by spaces in to a string.|
|6|ANGLE|Angle|Get the first 3 numbers separated by spaces from a string.|Get the 3 values and put them separated by spaces in to a string.|
|7|ENTITY|Entity|Get them by ID number|Get ID number from the Entity|
|8|ARRAY|Table|Spit string values are separated by spaces.|Put values into a string and separate them by spaces.|

## The example map
This is the official example map, so you can take it apart to see how it is used.

You don't have to ask for any permissions, you can always use parts or everything of the example map for everything you want. The *.vmf source file is included.

[Download gm_wiremapinterface.7z](http://www.solidfiles.com/d/36928e878f/)

**Happy mapping and wiring!**