**Contents**

1 Absolute  
2 Add  
3 And / Add  
4 Average  
5 Ceiling (Round up)  
6 Clamp  
7 Delta  
8 Delta (Rectified)  
9 Divide  
10 Exp  
11 Exponential Powers  
12 Floor (Round down)  
13 Identity (No change)  
14 Increment  
15 Increment/Decrement  
16 Inverse  
17 Log  
18 Log 10  
19 Modulo  
20 Multiply  
21 Negate  
22 Pi  
23 Percent  
24 Random  
25 Round  
26 Sign  
27 Square Root  
28 Subtract  

**Absolute**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Returns the absolute value of A  

**Add**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Adds the inputs together.  
Any amount of inputs can be used.  

**And / Add**  
Inputs: 	Type-Number A B  
Outputs: 	Type-Number Out  
Description: 	Outputs 0 if either input is negative or zero. Otherwise, outputs A + B.  

**Average**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Outputs the sum of the inputs divided by the number of inputs  

**Ceiling (Round up)**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs A rounded up to the nearest whole number  

**Clamp**  
Inputs: 	Type-Number A Min Max  
Outputs: 	Type-Number Out  
Description: 	Clamps A between Min and Max  

**Delta**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs the current value of A minus the previous value of A. This is updated whenever the value of A changes.  

**Delta (Rectified)**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs the current value of A minus the value of A at the previous tick.  
Modulo is applied to the output to prevent it from giving values outside the -180 to 180 range  

**Divide**  
Inputs: 	Type-Number A B  
Outputs: 	Type-Number Out  
Description: 	Divides A by B  

**Exp**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs [the number e](https://en.wikipedia.org/wiki/E_%28mathematical_constant%29) to the power of A  

**Exponential Powers**  
Inputs: 	Type-Number A B  
Outputs: 	Type-Number Out  
Description: 	Outputs A to the power of B  

**Floor (Round down)**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs A rounded down to the nearest whole number  

**Identity (No change)**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs A.  
Useful for organizing your wiring  

**Increment**  
Inputs: 	Type-Number A Clk Reset  
Outputs: 	Type-Number Out  
Description: 	Stores a number in memory, and always outputs that number. On the rising edge of Clk, A is added to  the stored number. On the rising edge of Reset, the stored number is reset to 0.  

**Increment/Decrement**  
Inputs: 	Type-Number A Increment Decrement Reset  
Outputs: 	Type-Number Out  
Description: 	Like Increment, but Clk is renamed to Increment, and Decrement is added. On the rising edge of  Decrement, A is subtracted from the stored number.  

**Inverse**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs 1 divided by A  

**Log**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs [the logarithm to the base e](https://en.wikipedia.org/wiki/Natural_logarithm) of A  

**Log 10**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs the logarithm to the base 10 of A  

**Modulo**  
Inputs: 	Type-Number A B  
Outputs: 	Type-Number Out  
Description: 	Outputs the remainder of A divided by B. Note: this can be negative if A is negative.  

**Multiply**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Multiplies all its inputs. You don't need to wire all the inputs if you don't need them.  

**Negate**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs A negated. (For example, 5 negated is -5. -2 negated is 2.  

**Pi**  
Inputs: 	None  
Outputs: 	Type-Number Out  
Description: 	Outputs Pi (3.14159...)  

**Percent**  
Inputs: 	Type-Number Value Max  
Outputs: 	Type-Number Out  
Description: 	Outputs what percentage Value is of Max. For example, 20 is 50% of 40, so this would output 50 if  Value was 20 and Max was 40.  

**Random**  
Inputs: 	Type-Number A B  
Outputs: 	Type-Number Out  
Description: 	Outputs a random number between A and B every tick  

**Round**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs A rounded to the nearest whole number  

**Sign**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs -1 when A is less than 0  

Outputs 0 when A is equal to 0  
Outputs 1 when A is greater than 0  

**Square Root**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Outputs the [square root](https://en.wikipedia.org/wiki/Square_root) of A  

**Subtract**  
Inputs: 	Type-Number A B  
Outputs: 	Type-Number Out  
Description: 	Outputs the B subtracted from A  
