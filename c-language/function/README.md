# Function

### Basic Concept of Function

* Functions receive either a fixed or variable amount of arguments.
* Functions can only return one value, or return no value.
* All C program has at least 1 function, which is `main().`All programs are allowed to define extra functions

### Define a function

{% tabs %}
{% tab title="Plain Text" %}
```c
return_type function_name( parameter list )
{
   body of the function
}

```
{% endtab %}

{% tab title="Example" %}
```c
/* 函数返回两个数中较大的那个数 */
int max(int num1, int num2) 
/*int is the return type, num1 & num2 are parameters,
max is the name of function*/
{
   /* 局部变量声明 */
   int result;
 
   if (num1 > num2)
      result = num1;
   else
      result = num2;
 
   return result; 
}
```
{% endtab %}
{% endtabs %}

A function consist of:

* Return type \(if no return, the return type will be void\)
* Name of the function
* Parameters
* Body of function

### Call/Reference a Function

```c
#include <stdio.h>
 
/* 函数声明 */
int max(int num1, int num2);
 
int main ()
{
   /* 局部变量定义 */
   int a = 100;
   int b = 200;
   int ret;
 
   /* 调用函数来获取最大值 */
   ret = max(a, b);
 
   printf( "Max value is : %d\n", ret );
 
   return 0;
}
 
/* 函数返回两个数中较大的那个数 */
int max(int num1, int num2) 
{
   /* 局部变量声明 */
   int result;
 
   if (num1 > num2)
      result = num1;
   else
      result = num2;
 
   return result; 
}
```

{% hint style="info" %}
Similar to defining a variable, when defining a function, it can be static and extern \(can be reference by program from other files\)
{% endhint %}

