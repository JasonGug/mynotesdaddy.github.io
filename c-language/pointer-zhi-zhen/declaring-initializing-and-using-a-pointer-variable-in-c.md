# Declaring, Initializing and using a pointer variable in C

### Declaration of C Pointer variable

Data type of a pointer must be same as the data type of the variable to which the pointer variable is pointing. `void` type pointer works with all data types, but is not often used.

```c
int *ip     // pointer to integer variable
float *fp;      // pointer to float variable
double *dp;     // pointer to double variable
char *cp;       // pointer to char variable
```

### Initialization of C Pointer variable

**Pointer Initialization** is the process of assigning address of a variable to a **pointer** variable. Pointer variable can only contain address of a variable of the same data type. In C language **address operator** `&` is used to determine the address of a variable. The `&` \(immediately preceding a variable name\) returns the address of the variable associated with it.

```c
#include<stdio.h>
    
void main()
{
    int a = 10;
    int *ptr;       //pointer declaration
    ptr = &a;       //pointer initialization
}
```

Pointer variable always point to variables of same datatype. Let's have an example to showcase this:

```c
#include<stdio.h>

void main()
{
    float a;
    int *ptr;
    ptr = &a;       // ERROR, type mismatch
}
```

If you are not sure about which variable's address to assign to a pointer variable while declaration, it is recommended to assign a `NULL` value to your pointer variable. A pointer which is assigned a `NULL` value is called a **NULL pointer**.

```c
#include <stdio.h>

int main() 
{
    int *ptr = NULL;
    return 0;
}
```

### Using the pointer or Dereferencing \(取消应用\) of Pointer

Once a pointer has been assigned the address of a variable, to access the value of the variable, pointer is **dereferenced**, using the **indirection operator** or **dereferencing operator** `*`.

```c
#include <stdio.h>

int main()
{
    int a, *p;  // declaring the variable and pointer
    a = 10;
    p = &a;     // initializing the pointer

    printf("%d", *p);    //this will print the value of 'a'

    printf("%d", *&a);   //this will also print the value of 'a'

    printf("%u", &a);    //this will print the address of 'a'

    printf("%u", p);     //this will also print the address of 'a'

    printf("%u", &p);    //this will print the address of 'p'
    
    return 0;
}
```

