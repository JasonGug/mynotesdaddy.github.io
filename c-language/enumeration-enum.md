# Enumeration \(enum\)

### Definition

Enum is a basic Data type to make data clearer & more readable.

### Example

```c
//Without Enum
#define MON  1
#define TUE  2
#define WED  3
#define THU  4
#define FRI  5
#define SAT  6
#define SUN  7

//With Enum
enum DAY
{
      MON=1, TUE, WED, THU, FRI, SAT, SUN
};
```

{% hint style="info" %}
第一个枚举成员的默认值为整型的 0，后续枚举成员的值在前一个成员上加 1。我们在这个实例中把第一个枚举成员的值定义为 1，第二个就为 2，以此类推。

First member of enum has a default value 0 and so on. However, if we set the first enum member to value 1, the second member will be 2 instead of 1 and so on.
{% endhint %}

```c
enum season {spring, summer=3, autumn, winter};

```

{% hint style="info" %}
In this case, spring is 0, summer is 3, autumn is 4, winter is 5.
{% endhint %}

### Define a Enum

There are 3 ways to define a enum:

```c
 //1: Define the enum then define Enum variable
 enum DAY
{
      MON=1, TUE, WED, THU, FRI, SAT, SUN
};
enum DAY day;

//2: Define the enum with the enum variable
enum DAY
{
      MON=1, TUE, WED, THU, FRI, SAT, SUN
} day;

//3: skip the enum name but define the enum variable
enum
{
      MON=1, TUE, WED, THU, FRI, SAT, SUN
} day;

//Full example
#include<stdio.h>
 
enum DAY
{
      MON=1, TUE, WED, THU, FRI, SAT, SUN
};
 
int main()
{
    enum DAY day;
    day = WED;
    printf("%d",day);
    return 0;
}
```

