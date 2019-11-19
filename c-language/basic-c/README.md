# Basic C



## Getting Started

```c
#include <stdio.h>

int main()
{
    /*My First C Program 我的第一个C程序*/
    printf("Hello World \n");
    
    return 0;
}
```

{% hint style="success" %}
`Hello, World!` \(Value in side the `printf()`function\) will be return 
{% endhint %}

* All C program must include function `main()`. The code start from `main()`.
* `/*......*/` is used for comment.
* `stdio.h` stands for Standard Input Output Header File \(标准输入输出头文件\). 
* `#include` is a Pre-Process Command \(预处理命令\)，used to import Header File. In this case, `stdio.h` When Compiler\(编译器\)  meet function `printf()`, if Header file`stdio.h` is not found, error will occur.
* `return 0` is the exit point of the program so the compiler knows that a new line has started.

