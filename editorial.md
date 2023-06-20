# The basic idea is the use of prefix sum.

## this problem reduces the time complexity from O(m*n)
## to O(n);

* instead of the dual for loop approach,
we used the concept of prefix sum.

we create an array of size n,initialise all its elements to 0;

Then , we add 1 to i1 element and subtract 1 from i2+1 element.

the prefix sum thus formed contains the actual happenings in the real world!!

then, find the max. of this prefix sum array!.
