Contents  

    Bitwise AND  
    Bitwise OR  
    Bitwise NOT  
    Bitwise XOR  
    Bit Shift Left  
    Bit Shift Right  

**Bitwise AND**  
Inputs: 	Type-Number  A B  
Outputs: 	Type-Number  Out  
Description: 	Bitwise AND takes two binary representations of equal length and performs the  
logical AND operation on each pair of corresponding bits.  

_Example:_  
`	0101 (decimal 5)`  
`AND	0011 (decimal 3)`  
`=	0001 (decimal 1)`  


**Bitwise OR**  
Inputs: 	Type-Number  A B  
Outputs: 	Type-Number  Out  
Description: 	Bitwise OR takes two bit patterns of equal length and performs the logical inclusive OR operation on  each pair of corresponding bits.  

_Example:_  
`	0101 (decimal 5)`  
`OR	0011 (decimal 3)`  
`=	0111 (decimal 7)`  


**Bitwise NOT**  
Inputs: 	Type-Number  A  
Outputs: 	Type-Number  Out  
Description: 	Bitwise NOT, or complement, is a unary operation that performs logical negation on each bit, forming   the ones' complement of the given binary value. Digits which were 0 become 1, and vice versa.  

_Example:_  
`NOT	0111 (decimal 7)`  
`=	1000 (decimal 8)`  


**Bitwise XOR**  
Inputs: 	Type-Number  A B  
Outputs: 	Type-Number  Out  
Description: 	A bitwise exclusive OR takes two bit patterns of equal length and performs the logical XOR operation   on each pair of corresponding bits. The result in each position is 1 if the two bits are different, and 0 if they are the same.  

_Example:_  
`	0101 (decimal 5)`  
`XOR	0011 (decimal 3)`  
`=	0110 (decimal 6)`  


**Bit Shift Left**  
Inputs: 	Type-Number  A B  
Outputs: 	Type-Number  Out  
Description: 	The bits of input A are shifted left by the amount of places of input B.  

_Example:_  
`	00010111	LEFT SHIFT BY ONE`  
`=	00101110`  


**Bit Shift Right**  
Inputs: 	Type-Number  A B  
Outputs: 	Type-Number  Out  
Description: 	The bits of input A are shifted right by the amount of places of input B.  

_Example:_  
`	00010111	RIGHT SHIFT BY TWO`  
`=	00000101`  
