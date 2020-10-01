**Contents**  

1 Add  
2 Clamp (angles)  
3 Clamp (numbers)  
4 Compose  
5 Decompose  
6 Delta  
7 Direction (Forward, Up, Right)  
8 Division  
9 Equal  
10 Identity  
11 Inequal  
12 Multiplication  
13 Multiplication (Components)  
14 Negate  
15 Normalize  
16 Round  
17 Select  
18 Shift Component Left  
19 Shift Component Right  
20 Subtraction  
21 To String  

**Add**  
Inputs: 	![Angle](Type-Angle.png "Angle") A B C D E F G H  
Outputs: 	![Angle](Type-Angle.png "Angle") Out  
Description: 	Adds the inputs together.  

**Clamp (angles)**  
Inputs: 	Type-Angle A Min Max  
Outputs: 	Type-Angle Out  
Description: 	Clamps each angle component from A between their counterparts of Min and Max.  

**Clamp (numbers)**  
Inputs: 	Type-Angle A Type-Number Min Max  
Outputs: 	Type-Angle Out  
Description: 	Clamps each angle component from A between the values of Min and Max.  

**Compose**  
Inputs: 	Type-Number Pitch Yaw Roll  
Outputs: 	Type-Angle Out  
Description: 	Creates an angle from the inputs Pitch Yaw and Roll.  

**Decompose**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Number Pitch Yaw Roll  
Description: 	Outputs the components from A as Pitch Yaw and Roll.  

**Delta**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Outputs the current value of A minus the value of A at the previous tick.  

**Direction (Forward, Up, Right)**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Vector Forward Up Right  
Description: 	Outputs 3 directional vectors representing the angle components.  

**Division**  
Inputs: 	Type-Angle A B  
Outputs: 	Type-Angle Out  
Description: 	Divides angle A by B.  

**Equal**  
Inputs: 	Type-Angle A B  
Outputs: 	Type-Number Out  
Description: 	Outputs 1 when inputs A and B are equal, 0 when they are unequal.  

**Identity**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Outputs A.  
Useful for organizing your wiring.  

**Inequal**  
Inputs: 	Type-Angle A B  
Outputs: 	Type-Number Out  
Description: 	Outputs 0 when inputs A and B are equal, 1 when they are unequal.  

**Multiplication**  
Inputs: 	Type-Angle A B  
Outputs: 	Type-Angle Out  
Description: 	Multiplies angle A and B  

**Multiplication (Components)**  
Inputs: 	Type-Angle A B  
Outputs: 	Type-Angle Out  
Description: 	Multiplies the components of angle A and B.  

**Negate**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Negates angle A.  

**Normalize**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Normalizes angle A.  

**Round**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Rounds angle A to integers.  

**Select**  
Inputs: 	Type-Number Select Type-Angle A B C D E F G H  
Outputs: 	Type-Angle Out  
Description: 	Outputs the selected angle.  

**Shift Component Left**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Outputs the components shifted left; Pitch = Yaw , Yaw = Roll and Roll = Pitch.  

**Shift Component Right**  
Inputs: 	Type-Angle A  
Outputs: 	Type-Angle Out  
Description: 	Outputs the components shifted right; Pitch = Roll , Yaw = Pitch and Roll = Yaw.  

**Subtraction**  
Inputs: 	Type-Angle A B  
Outputs: 	Type-Angle Out  
Description: 	Subtracts angle B from A.  

**To String**  
Inputs: 	Type-Angle A  
Outputs: 	Type-String Out  
Description: 	Outputs the angle as a string, "[ Pitch , Yaw , Roll ]".  
