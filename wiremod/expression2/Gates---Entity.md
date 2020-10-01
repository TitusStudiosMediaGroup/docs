Contents

    1 AimDirection
    2 AimEntity
    3 AimNormal
    4 AimPosition
    5 Angles
    6 Angular Velocity
    7 Angular Velocity (vector)
    8 Apply Angular Force
    9 Apply Force
    10 Apply Offset Force
    11 Apply Torque
    12 Bearing
    13 Class
    14 Color
    15 Direction - (forward, right, up)
    16 Driver
    17 Elevation
    18 Entity ID
    19 Equal
    20 Heading
    21 Health
    22 ID to Entity
    23 Inequal
    24 Inertia
    25 Is in vehicle
    26 Is NPC
    27 Is on fire
    28 Is on ground
    29 Is player
    30 Is player holding
    31 Is under water
    32 valid
    33 Is vehicle
    34 Is weapon
    35 Is world
    36 Local to world
    37 Mass
    38 Mass center
    39 Mass center (local)
    40 material
    41 Model
    42 Name
    43 Owner
    44 Position
    45 Radius
    46 Select
    47 Set color
    48 Set mass
    49 SteamID
    50 Time connected
    51 Velocity
    52 Velocity (local)
    53 World to local (angle)
    54 World to local (vector)

AimDirection
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the aim direction of the player / npc as a normalized vector.



AimEntity
Inputs: 	Type-Entity Ent
Outputs: 	Type-Entity Out
Description: 	Outputs the entity where the player / npc is aiming at.



AimNormal
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the a normalized vector perpendicular to the surface where the player / npc is aiming at.



AimPosition
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the position of where the player / npc is aiming at as a vector.



Angles
Inputs: 	Type-Entity Ent
Outputs: 	Type-Angle Out
Description: 	Outputs the angles of the entity.



Angular Velocity
Inputs: 	Type-Entity Ent
Outputs: 	Type-Angle Out
Description: 	Outputs the angular velocity of the entity.



Angular Velocity (vector)
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the angular velocity of the entity as vector.



Apply Angular Force
Inputs: 	Type-Entity Ent Type-Angle Ang
Outputs: 	Type-Number Out
Description: 	Applies the inputted angle as angular force to the entity



Apply Force
Inputs: 	Type-Entity Ent Type-Vector Vec
Outputs: 	Type-Number Out
Description: 	Applies the inputted vector as force to the entity



Apply Offset Force
Inputs: 	Type-Entity Ent Type-Vector Vec Offset
Outputs: 	Type-Number Out
Description: 	Applies the input Vec as force on the entity, at input Offset as world position



Apply Torque
Inputs: 	Type-Entity Ent Type-Vector Vec
Outputs: 	Type-Number Out
Description: 	Applies the input Vec as torque on the entity



Bearing
Inputs: 	Type-Entity Entity Type-Vector Position Type-Number Clk
Outputs: 	Type-Number Out
Description: 	Outputs the bearing between the aim direction of player / npc and the position vector
Updated when input Clk is changed.



Class
Inputs: 	Type-Entity Entity
Outputs: 	Type-String Out
Description: 	Outputs the class of the entity as string.



Color
Inputs: 	Type-Entity Entity
Outputs: 	Type-Vector Out
Description: 	Outputs the color of the entity as vector.



Direction - (forward, right, up)
Inputs: 	Type-Entity Entity
Outputs: 	Type-Vector Forward Right Up
Description: 	Outputs 3 normalized vectors representing the forward right and up direction of the entity



Driver
Inputs: 	Type-Entity Entity
Outputs: 	Type-Vector Entity
Description: 	Outputs the driver of an vehicle entity.



Elevation
Inputs: 	Type-Entity Entity Type-Vector Position Type-Number Clk
Outputs: 	Type-Number Out
Description: 	Outputs the elevation between the aim direction of player / npc and the position vector
Updated when input Clk is changed.



Entity ID
Inputs: 	Type-Entity Entity
Outputs: 	Type-Number Out
Description: 	Outputs the ID of an entity as number.



Equal
Inputs: 	Type-Entity A B
Outputs: 	Type-Number Out
Description: 	Outputs 1 is A is the same entity as B, 0 when it isn't



Heading
Inputs: 	Type-Entity Entity Type-Vector Position Type-Number Clk
Outputs: 	Type-Number Out
Description: 	Outputs the heading as angle between the aim direction of player / npc and the position vector
Updated when input Clk is changed.



Health
Inputs: 	Type-Entity Entity
Outputs: 	Type-Number Out
Description: 	Outputs the health of an entity as number.



ID to Entity
Inputs: 	Type-Number A
Outputs: 	Type-Entity Entity
Description: 	Outputs the entity which has an ID as A, returns null entity when not found.



Inequal
Inputs: 	Type-Entity A B
Outputs: 	Type-Number Out
Description: 	Outputs 0 is A is the same entity as B, 1 when it isn't



Inertia
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the inertia of an entity as vector.



Is in vehicle
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the player is in a vehicle, 0 when not.



Is NPC
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is a NPC, 0 when not.



Is on fire
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is on fire, 0 when not.



Is on ground
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is standing on a solid surface, 0 when not.
This also works on props.



Is player
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is a player, 0 when not.



Is player holding
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is being held by an player, 0 when not.
Works with hands, gravgun and physgun.



Is under water
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is under water, 0 when not.



valid
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is a valid, 0 when not.



Is vehicle
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is a vehicle, 0 when not.



Is weapon
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is a weapon, 0 when not.



Is world
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs 1 when the entity is a the world, 0 when not.



Local to world
Inputs: 	Type-Entity Ent Type-Vector Vec
Outputs: 	Type-Vector Out
Description: 	Outputs a position local to the entity as world position.



Mass
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs the mass of an entity as number.



Mass center
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the mass center of an entity as world vector.



Mass center (local)
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the mass center of an entity as local vector.



material
Inputs: 	Type-Entity Ent
Outputs: 	Type-String Out
Description: 	Outputs the material of an entity as string.



Model
Inputs: 	Type-Entity Ent
Outputs: 	Type-String Out
Description: 	Outputs the model of an entity as string.



Name
Inputs: 	Type-Entity Ent
Outputs: 	Type-String Out
Description: 	Outputs the name of an entity as string.



Owner
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs the owner of entity as entity.



Position
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the position of an entity as world vector.



Radius
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs the approximate radius of an entity as number.



Select
Inputs: 	Type-Entity A B C D E F G H Type-Number Choice
Outputs: 	Type-Entity Out
Description: 	Outputs the entity selected by the Choice input.



Set color
Inputs: 	Type-Entity Ent Type-Vector Col
Outputs: 	Type-Entity Out
Description: 	Sets the color of the Entity.



Set mass
Inputs: 	Type-Entity Ent Type-Number Mass
Outputs: 	Type-Number Out
Description: 	Sets the mass of the Entity.



SteamID
Inputs: 	Type-Entity Ent
Outputs: 	Type-String Out
Description: 	Outputs the SteamID of an entity as string.



Time connected
Inputs: 	Type-Entity Ent
Outputs: 	Type-Number Out
Description: 	Outputs the time that the player has been connected in seconds.



Velocity
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the velocity of an entity as world vector.



Velocity (local)
Inputs: 	Type-Entity Ent
Outputs: 	Type-Vector Out
Description: 	Outputs the velocity of an entity as local vector.



World to local (angle)
Inputs: 	Type-Entity Ent Type-Angle Ang
Outputs: 	Type-Angle Out
Description: 	Outputs a world angle as local angle to the entity.



World to local (vector)
Inputs: 	Type-Entity Ent Type-Vector Vec
Outputs: 	Type-Vector Out
Description: 	Outputs a world vector as local vector to the entity.
