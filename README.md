# FCALtoC
A translator that takes a domain specific language, the FCAL (Forest Cover Analysis Language) code and converts it to proper C++ code.
The project was developed using the iterative model of development, with a total of 4 iterations. 
Automated testing (CXXTest - the unit testing framework) was also used to ensure for correctness.

The translator is primarily made up of:
Scanner (Regex Matching and token generation)
Parser (Takes the linked list of tokens and creates nodes for the AST)
AST (Abstract Syntax Tree that holds all the nodes in the proper hierarchy)
On a high level, the scanner generates the list of tokens, which the parser will convert into nodes and form the AST, and then 'translate' the code into a C++ equivalent during the unparsing.
