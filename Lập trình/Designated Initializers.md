# In C
## Arrays
You can choose which element of the array to be initialized. For example,
```c
double A[5] = { [0] = 9.0, [3] = 3.4, };
```
**Special rule:** Any position which is not listed in the declaration is set to 0. So in the example `A[1]`  is filled with 0.

{0} is a valid initializer for all object types that are not [[Variable-length Arrays]]. This will initalize all the elements to 0.