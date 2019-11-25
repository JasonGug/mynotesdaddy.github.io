# Function Pointer

### How to define a function pointer

```c
#include <stdio.h>
 
int max(int x, int y) //Define a function
{
    return x > y ? x : y;
}
 
int main(void)
{
    int (* p)(int, int) = & max; // Define the funtion pointer. 
    //& symbol can be removed
    int a, b, c, d;
 
    printf("请输入三个数字:");
    scanf("%d %d %d", & a, & b, & c);
 
    /* 与直接调用函数等价，d = max(max(a, b), c) */
    d = p(p(a, b), c); 
 
    printf("最大的数字是: %d\n", d);
 
    return 0;
}
```

