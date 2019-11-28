---
description: 此篇笔记为全中文 方便理解 大多数代码基于JavaScript而不是C 因为js会大量使用回调函数 利于应用
---

# Callback Function

### What is callback function

A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action.

{% hint style="info" %}
打个比方，有一家旅馆提供叫醒服务，但是要求旅客自己决定叫醒的方法。可以是打客房电话，也可以是派服务员去敲门，睡得死怕耽误事的，还可以要求往自己头上浇盆水。这里，“叫醒”这个行为是旅馆提供的，相当于库函数，但是叫醒的方式是由旅客决定并告诉旅馆的，也就是回调函数。而旅客告诉旅馆怎么叫醒自己的动作，也就是把回调函数传入库函数的动作，称为**登记回调函数**（to register a callback function）。
{% endhint %}

让我用人话解释一下，回调函数是一个函数，将会在另一个函数完成执行后立即执行。  
回调函数是一个作为参数传给另一个 JavaScript 函数的函数。这个回调函数会在传给的函数内部执行。  
在 JavaScript 中函数被看作是一类对象（Object）。对于一类对象，我们的意思是指数字、函数或变量可以与语言中的其他实体相同。作为一类对象，可以将函数作为变量传给其他函数，也可以从其他函数中返回这些函数。

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

