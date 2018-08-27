## PEP 8 Style guide

### General Rules: 
* 4 spaces per indention level  
* For long function names, use hanging indent to distinguish variables from rest  
* Spaces are preferred over tabs  
* Line breaks before binary operations  
* 2 blank lines around top-level function and class definitions, 1 around methods  
* All module imports should be on separate lines  
* Avoid wildcard import (from x import *)  
* " and ' are the same in python, pick a rule.  But use """ for comment lines  
* Comments should be complete sentences  
* Use ''.startswith() and ''.endswith() instead of string slicing to check for prefixes or suffixes. (i.e. if foo.startswith('bar') )
* For sequences, (strings, lists, tuples), use the fact that empty sequences are false


### Whitespaces:  
No white-space 
* immediately inside parentheses, brackets, or braces
* After trailing comma
* Before a comma, semicolon, or colon
* Immediately before the open parenthesis
* Trailing anything
* Surrounding higher propriety operators when mixed with lower propriety (i.e. c = (a+b) * (a-b), x = x*2 - 1 )
* Around = when defining default parameter

Intentional White-spaces
* Surrounding binary operators (=, +=, -= etc., ==, <, >, !=, <>, <=, >=, in, not in, is, is not, and, or, not)

### Naming conventions:

| Component | Convention |
| --------- | ---------  |
| Package and Module | lowercase |
| Class | CamelCase |
| Type Variable | CamelCase |
| Exception | ErrorCamelCase |
| Global Variable | lower_case |
| Method Name | lower_case |
| Constants | ALL_CAPS |

[Back to Python page](../python.md)
