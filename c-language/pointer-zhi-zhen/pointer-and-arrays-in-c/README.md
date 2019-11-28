# Pointer and Arrays in C

### Basic Explanation

When an array is declared, compiler allocates sufficient amount of memory to contain all the elements of the array. Base address i.e address of the first element of the array is also allocated by the compiler. 

Assume we declare an array `arr`,

```c
int arr[5] = { 1, 2, 3, 4, 5 };
```

Assuming that the base address of `arr` is 1000 and each integer requires two bytes, the five elements will be stored as follows:

![Example of each element&apos;s address](../../../.gitbook/assets/image%20%288%29.png)

Here variable `arr` will give the base address, which is a constant pointer pointing to the first element of the array, `arr[0]`. Hence `arr` contains the address of `arr[0]` i.e `1000`. In short, `arr` has two purpose :

* it is the **name** of the array 
* it **acts as a pointer pointing towards the first element in the array.**

Therefore, `arr` is equal to `&arr[0]` by default. We can also declare a pointer of type `int` to point to the array `arr`.

```c
int *p;
p = arr;  
// or, 
p = &arr[0];    //both the statements are equivalent.

p++; //move to next element
p--; //back to previous element
```



