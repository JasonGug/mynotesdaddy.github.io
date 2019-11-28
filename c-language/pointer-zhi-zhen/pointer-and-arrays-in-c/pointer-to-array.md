# Pointer to Array

As studied above, we can use a pointer to point to an array, and then we can use that pointer to access the array elements. Lets have an example:

```c
#include <stdio.h>

int main()
{
    int i;
    int a[5] = {1, 2, 3, 4, 5};
    int *p = a;     // same as int*p = &a[0]
    for (i = 0; i < 5; i++)
    {
        printf("%d", *p); 
        // Print all the values stored in the array one by one
        p++;
    }
    
    return 0;
}
```

In the above program, the pointer `*p` will print all the values stored in the array one by one. We can also use the Base address \(`a` in above case\) to act as a pointer and print all the values.

Replacing the `printf("%d", *p)` statement of above example:

```c
printf("%d", *p); //Print all the values stored in the array one by one

printf("%d", p); //Print all the address of each element one by one

printf("%d", a[i]); //Print the values stored in the array by incrementing index

printf("%d", i[a]); //Same as above (a[i]) 

printf("%d", a+i); //This will print address of all the array elements

printf("%d", *(a+i)); //Print the vlaues of array element
// *(a+i) is same as a[i]

printf("%d", *a); //Print value of a[0] only

a++ // Compile time error, we can't change base address of the array
```



