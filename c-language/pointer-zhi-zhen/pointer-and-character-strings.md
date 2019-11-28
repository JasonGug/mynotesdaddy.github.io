# Pointer and Character strings

### String Pointer

Pointer can also be used to create strings. Pointer variables of `char` type are treated as string.

```c
char *str = "Hello";
```

The above code creates a string and stores its address in the pointer variable `str`. The pointer `str` now points to the first character of the string "Hello". Another important thing to note here is that the string created using `char` pointer can be assigned a value at **runtime**.

```c
char *str;
str = "hello";      //this is Legal
```

The content of the string can be printed using `printf()` and `puts()`.

```c
printf("%s", str);
puts(str);
```

Notice that `str` is pointer to the string, it is also name of the string. Therefore we do not need to use indirection operator `*`.

### Array of Pointer

We can also have array of pointers. Pointers are very helpful in handling character array with rows of varying length.

```c
char *name[3] = { 
    "Adam",
    "chris",
    "Deniel"
};
//Now lets see same array without using pointer
char name[3][20] = { 
    "Adam",
    "chris",
    "Deniel"
};
```

![Difference between pointer &amp; no-pointer](../../.gitbook/assets/image%20%284%29.png)

In the second approach memory wastage is more, hence it is preferred to use pointer in such cases.

When we say memory wastage, it doesn't means that the strings will start occupying less space, no, characters will take the same space, but when we define array of characters, a contiguous memory space is located equal to the maximum size of the array, which is a wastage, which can be avoided if we use pointers instead.

