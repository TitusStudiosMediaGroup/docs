Contents

    1 D-Latch
    2 Latch (Edge triggered)
    3 RAM
    4 RS-Latch
    5 SR-Latch
    6 Toggle (Edge triggered)
    7 Toggle While(Edge triggered)
    8 Up/Down Counter
    9 Write Only Memory(4 store)

D-Latch
Inputs: 	Type-Number.png Data Clk
Outputs: 	Type-Number.png Out
Description: 	The D-Latch will keep updating as long as its Clk input is positive. It outputs whatever value is currently stored.



Latch (Edge triggered)
Inputs: 	Type-Number.png Data Clk
Outputs: 	Type-Number.png Out
Description: 	The Latch is Edge-Triggered, meaning that it only stores the value when the Clk input changes from 0 to positive. In order to change the data stored, the Clk input must go back to zero or negative and then back to positive. The Latch will output whatever value is currently stored.



RAM
Inputs: 	Type-Number.png Data AddrRead AddrWrite Clk Reset
Outputs: 	Type-Number.png Out
Description: 	These memory chips works like a row of data, where you specify the address you want to write to (and the address you want to read from).
Remember: The row starts with zero: 0, 1, 2, 3, 4 and so on. This concept is very similar to arrays in programming.



RS-Latch
Inputs: 	Type-Number.png S R
Outputs: 	Type-Number.png Out
Description: 	SR is short for "Set-Reset". The chip keeps the first value input to S. When R is positive, the value of S is reset.



SR-Latch
Inputs: 	Type-Number.png S R
Outputs: 	Type-Number.png Out
Description: 	Same as RS-Latch, The difference is that each input has to 0 in order for the other to work.



Toggle (Edge triggered)
Inputs: 	Type-Number.png Clk OnValue OffValue
Outputs: 	Type-Number.png Out
Description: 	This chip toggles between two values when its Clk input is positive. Its OffValue and OnValue inputs specify these two values. Like the Latch, the Toggle chip is also Edge-Triggered. When created, the Toggle chip begins Off.



Toggle While(Edge triggered)
Inputs: 	Type-Number.png Clk OnValue OffValue
Outputs: 	Type-Number.png Out
Description: 	This chip toggles between two values when its Clk input is positive. Its OffValue and OnValue inputs specify these two values. Like the Latch, the Toggle chip is also Edge-Triggered. When created, the Toggle chip begins Off. As addition While has to be 1 in order to toggle to the OnValue.



Up/Down Counter
Inputs: 	Type-Number.png Clk Increment Decrement Reset
Outputs: 	Type-Number.png Out
Description: 	When Clk is triggered, outputs 1 when Increment is 1, outputs 0 when Decrement is 1. Doesn't do anything when Increment and Decrement are equal.



Write Only Memory(4 store)
Inputs: 	Type-Number.png Data AddrWrite Clk
Outputs: 	Type-Number.png Out
Description: 	Use this gate to store secret data which you don't want anyone to read, including yourself.