---
description: 此篇笔记为全中文 方便理解 大多数代码基于JavaScript而不是C 因为js会大量使用回调函数 利于应用
---

# Callback Function

### What is callback function

A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.

![Architecture of callback function](../../.gitbook/assets/image%20%282%29.png)

### C Example

```c
#include <stdlib.h>  
#include <stdio.h>
 
// This is the function we are goi
void populate_array(int *array, size_t arraySize, int (*getNextValue)(void))
{
    for (size_t i=0; i<arraySize; i++)
        array[i] = getNextValue();
}
 
// 获取随机值
int getNextRandomValue(void)
{
    return rand();
}
 
int main(void)
{
    int myarray[10];
    populate_array(myarray, 10, getNextRandomValue);
    for(int i = 0; i < 10; i++) {
        printf("%d ", myarray[i]);
    }
    printf("\n");
    return 0;
}


/*16807 282475249 1622650073 984943658 1144108930
470211272 101027544 1457850878 1458777923 2007237709*/

```

