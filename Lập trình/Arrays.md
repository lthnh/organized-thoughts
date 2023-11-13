# Arrays in C
Arrays are not pointers.

These two declarations declare variable of exactly the same types.
```c
double A[m][n];
double (B[m])[n];
```
Both `A` and `B` are `m` objects of array type `double[n]`.

We can use [[Designated Initializers]] to make robust declarations.