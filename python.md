# Python Stuff I Regularly Use
[Styling](#pep-8-style-guide)
[Formatted Output](#Formatted-output)
[Logging](#logging)
[Arrayfire](#arrayfire)

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
| ----      | ----       |
| Package and Module | lowercase |
| Class | CamelCase |
| Type Variable | CamelCase |
| Exception | ErrorCamelCase |
| Global Variable | lower_case |
| Method Name | lower_case |
| Constants | ALL_CAPS |

[Back to Top](#)

## Formatted output
`%[flags][width][.precision]type` 

| Flags	| Meaning |
|---		|---		|
| #		| Used with o, x or X specifiers the value is preceded with 0, 0o, 0O, 0x or 0X respectively. |
| 0		| The conversion result will be zero padded for numeric values. |
| -		| The converted value is left adjusted |
|  		| If no sign (minus sign e.g.) is going to be written, a blank space is inserted before the value. |
| +		| A sign character ("+" or "-") will precede the conversion (overrides a "space" flag). |

| Type	| Meaning |
|---		|---		|
| d		| Signed integer decimal.	|
| i		| Signed integer decimal.	|
| o		| Unsigned octal.	|
| u		| Obsolete and equivalent to 'd', i.e. signed integer decimal.	|
| x		| Unsigned hexadecimal (lowercase).	|
| X		| Unsigned hexadecimal (uppercase).	|
| e		| Floating point exponential format (lowercase).	|
| E		| Floating point exponential format (uppercase).	|
| f		| Floating point decimal format.	|
| F		| Floating point decimal format.	|
| g		| Same as "e" if exponent is greater than -4 or less than precision, "f" otherwise.	|
| G		| Same as "E" if exponent is greater than -4 or less than precision, "F" otherwise.	|
| c		| Single character (accepts integer or single character string).	|
| r		| String (converts any python object using repr()).	|
| s		| String (converts any python object using str()).	|
| %		| No argument is converted, results in a "%" character in the result.	|

[All this is taken from here.](https://www.python-course.eu/python3_formatted_output.php)
[Back to Top](#)


## Logging
Setting up a new logger
```
import logging
logger=logging.getLogger("loggerName")
```

| Level 		| Numeric Value 	| Python Call 	|
| ---- 		| ---- 			| ---- 		|
| CRITICAL 	| 50 			| critical 	|
| ERROR 		| 40 			| error 		|
| WARNING 	| 30 			| warning 	|
| INFO 		| 20 			| info  		|
| DEBUG 		| 10 			| debug  		|
| NOTSET 		|  0 			|  			|

[Back to Top](#)

## [Arrayfire](http://arrayfire.org/arrayfire-python/index.html)

### algorithm
Count number of non-zero elements in an array along a specified dimeinsion.  
`count(a, dim=None)`

Check if any the elements along a specified dimension are true.  
`any_true(a, dim=None)`

Find the maximum value of all the elements along a specified dimension.
`max(a, dim=None)`

Find the minimum value of all the elements along a specified dimension.
`arrayfire.algorithm.min(a, dim=None)`

Sort the array along a specified dimension.  
`sort(a, dim=0, is_ascending=True)`

Find the unique elements of an array.  
`set_unique(a, is_sorted=False)`

### array
Displays the contents of an array.  
`display(a, precision=4)`

### arith
Raise 2 to the power of each element in input.
`pow2(a)`


### data
Select elements from one of two arrays based on condition.  
`replace(lhs, cond, rhs)`

Select elements from one of two arrays based on condition.  
`select(cond, lhs, rhs)`

Join two or more arrayfire arrays along a specified dimension.  
`join(dim, first, second, third=None, fourth=None)`

### device

### statistics
`mean(a, weights=None, dim=None)`
