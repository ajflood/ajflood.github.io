# Python Stuff I Regurally Use

## Logging.
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


## Arrayfire

### algorithm
Count number of non-zero elements in an array along a specified dimeinsion.  
`count(a, dim=None)`

Check if any the elements along a specified dimension are true.  
`any_true(a, dim=None)`

### arith

### data
Select elements from one of two arrays based on condition.  
`replace(lhs, cond, rhs)`

Select elements from one of two arrays based on condition.  
`select(cond, lhs, rhs)`

### device

