# Pointer of Multidimensional Array



A multidimensional array is of form, `a[i][j]`. Lets see how we can make a pointer point to such an array. As we know now, name of the array gives its base address. In `a[i][j]`, `a` will give the base address of this array, even `a + 0 + 0` will also give the base address, that is the address of `a[0][0]` element.

Here is the generalized form for using pointer with multidimensional arrays.

```c
*(*(a + i) + j)
```

which is same as,

```c
a[i][j]
```

