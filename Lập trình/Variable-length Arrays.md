# In C
Since every valid pointer is assumed to refer to the first element of an array of the reference type, you can just allocate an arbitrary amount of memory for the pointer.

This can be considered VLA in C cause you can just reallocate the amount 
memory associated with the pointer to the amount that you need. 

 Keep it mind that the abuse of [[realloc()]] function can lead to memory problems. For example the [[Query the document]] problem.