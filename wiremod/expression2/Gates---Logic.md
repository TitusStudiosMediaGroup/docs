Logic gates are the standard digital logic gates you can find on a circuit board. They all do simple binary tasks, and therefore only have one output.  

**Contents**  

    OR  
    AND  
    NOT  
    NAND  
    NOR  
    XOR  
    XNOR  

**OR**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Returns 1 if any input is 1. Returns 0 if no inputs are 1.  
Truth Table  
`Input 1	Input 2	Output`  
`0	0	0`  
`1	0	1`  
`1	1	1`  

**AND**  
Inputs: 	Type-Number.png A B C D E F G H  
Outputs: 	Type-Number.png Out  
Description: 	Returns 1 only if all inputs are 1, otherwise returns 0.  
Truth Table  
`Input 1	Input 2	Output`  
`0	0	0`  
`1	0	0`  
`1	1	1`  

**NOT**  
Inputs: 	Type-Number A  
Outputs: 	Type-Number Out  
Description: 	Returns 1 if input is 0. Returns 0 if input is 1.  
Truth Table  
`Input	Output`  
`0	1`  
`1	0`  

**NAND**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Equivalent to adding a NOT to an AND. Returns 0 if all inputs are 1. Returns 1 if any inputs are 0.  
Truth Table  
`Input 1	Input 2	Output`  
`0	0	1`  
`1	0	1`  
`1	1	0`  

**NOR**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Equivalent to adding a NOT to an OR. Returns 0 if any inputs are 1. Returns 1 if all inputs are 0.  
Truth Table  
`Input 1	Input 2	Output`  
`0	0	1`  
`1	0	0`  
`1	1	0`  

**XOR**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Exclusive OR. Returns 1 if only one input is 1. Returns 0 if all inputs are 0 or more than one input is 1.  
Truth Table  
`Input 1	Input 2	Output`  
`0	0	0`  
`1	0	1`  
`1	1	0`  

**XNOR**  
Inputs: 	Type-Number A B C D E F G H  
Outputs: 	Type-Number Out  
Description: 	Equivalent to adding a NOT to an XOR. Returns 0 if only one input is 1. Returns 1 if all inputs are 0 or more than one input is 1.  
Truth Table  
`Input 1	Input 2	Output`  
`0	0	1`  
`1	0	0`  
`1	1	1`  