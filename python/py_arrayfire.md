## [Arrayfire](http://arrayfire.org/arrayfire-python/index.html)

### This error means you ran out of memory

`IndexError: In function af_err af_assign_seq(void**, af_array, unsigned int, const af_seq*, af_array)
In file src/api/c/assign.cpp:147`

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

When cond==T select lhs, when cond==F select rhs)
`select(cond, lhs, rhs)`



[Back to Python page](../python.md)
