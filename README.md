# 2D array as 1D
Let *A* be a two-dimensional array with *r* rows and *c* columns with indices i and j, representing a_{ij} in A
We can construct a one-dimenional array A' from A by letting the index i' = c*i + j for all i,j.
Conversely we can obtain the indices of *A* by letting i=i' / c and j=i' % c.

# 2D sub-array as 1D
Utilizing the above concept let us construct a matrix *A'* from
```
00 01 02 03 04
05 06 07 08 09
10 11 12 13 14
15 16 17 18 19
```
Given the sub array S \in A', with column c' and rows r':
```
06 07 08
11 12 13
```

we can obtain its indices from its starting point in *A'* (1,1) by:

k=c(i+1) + (j+1)

and in general a sub array can be obtained by:

k=c(i+i') + (j+j')
