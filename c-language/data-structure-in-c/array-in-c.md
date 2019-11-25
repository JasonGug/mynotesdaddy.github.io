# Array in C

### Definition

Arrays are special variables which can hold more than one value under the same variable name, organised with an index. Arrays are defined using a very straightforward syntax.

```c
/* defines an array of 10 integers */
int numbers[10];

/* defines an array of 5 doubles */
double balance[5];

```

### Initialize an Array

There are 2 ways to initialize an array

```c
int numbers[10];

/* populate the array */
numbers[0] = 10;
numbers[1] = 20;
numbers[2] = 30;
numbers[3] = 40;
numbers[4] = 50;
numbers[5] = 60;
numbers[6] = 70;

//OR

int number[10] = { 10 , 20 , 30 , 40 , 50 , 60 , 70 };
```

Traverse an Array

```c
#include <stdio.h>
 
int main ()
{
   int n[ 10 ]; /* n 是一个包含 10 个整数的数组 */
   int i,j;
 
   /* 初始化数组元素 */         
   for ( i = 0; i < 10; i++ )
   {
      n[ i ] = i + 100; /* 设置元素 i 为 i + 100 */
   }
   
   /* 输出数组中每个元素的值 */
   for (j = 0; j < 10; j++ )
   {
      printf("Element[%d] = %d\n", j, n[j] );
   }
 
   return 0;
}
```

