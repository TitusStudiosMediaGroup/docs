**Contents**  

    Value retriever  
    8x merger  
    8x splitter  
    8x splitter  

**Value Retriever**  
Inputs: 	Type-Number  Index Type-Array  Tbl  
Outputs: 	Type-Number  Out  
Description: 	Outputs the index number in the array that is equal to Index.  

**8x Merger**  
Inputs: 	Type-Number  A B C D E F G H  
Outputs: 	Type-Array  Tbl  
Description: 	Takes eight values and turns into a array.  

**8x Splitter**  
Inputs: 	Type-Array  Tbl  
Outputs: 	Type-Number  A B C D E F G H  
Description: 	Splits array data up in eight outputs.  

**8x Splitter**  
Inputs: 	Type-Number  A B C D E F G H Type-Array  Tbl (BiDi)  
Outputs: 	Type-Number  A B C D E F G H Type-Array  Tbl (BiDi)  
Description: 	Like the merger and the splitter in one gate, but it only works with another "Bidirectional Array".  
This means that two duplexer's can both send and receive data from each other.  
