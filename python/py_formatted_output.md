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
[Back to Python page](../python.md)
