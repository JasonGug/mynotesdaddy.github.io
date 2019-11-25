# Declare \(声明\) vs. Define \(定义\)

## Defining/Declaring Variable

Defining: Used for variable to distribute the space and initialize the variable. In C, 1 variable can only be defined once.

Declaring: Used for program to acknowledge the variable type and name

Defining is Declaring BUT `extern` Declaring is not defining

```c
/*Declare variables*/

extern int d = 3, f = 5;    // d 和 f 的声明与初始化

/*Define variables without initialisation*/
int    i, j, k; 
char   c, ch;
float  f, salary;
double d;

/*Define variables with initialisation*/
int d = 3, f = 5;           // 定义并初始化 d 和 f
byte z = 22;                // 定义并初始化 z
char x = 'x';               // 变量 x 的值为 'x'
```

## Example

```c
#include <stdio.h>
 
//Define x, y outside the function
int x;
int y;
int addtwonum()
{
    // Declare that variable x & y is external variable.
    extern int x;
    extern int y;
    // Assign value to x & y
    x = 1;
    y = 2;
    return x+y;
}
 
int main()
{
    int result;
    // call function addtwonum()
    result = addtwonum();
    
    printf("result is: %d",result);
    return 0; //result is 3
}
```

