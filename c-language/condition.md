# Condition

### if...else in C

```c
if(boolean_expression)
{
   /* 如果布尔表达式为真将执行的语句 */
}
```

### switch in C

```c
#include <stdio.h>
 
int main ()
{
   /* 局部变量定义 */
   char grade = 'B';
 
   switch(grade)
   {
   case 'A' :
      printf("很棒！\n" );
      break;
   case 'B' :
   case 'C' :
      printf("做得好\n" );
      break;
   case 'D' :
      printf("您通过了\n" );
      break;
   case 'F' :
      printf("最好再试一下\n" );
      break;
   default :
      printf("无效的成绩\n" );
   }
   printf("您的成绩是 %c\n", grade );
 
   return 0;
}
```

### Ternary Operator

This can replace if...else... to make coding much clearer.  
FORMAT: **Condition ? ifTure : ifFalse**;

```c
//Condition ? ifTrue : ifFalse;

#include<stdio.h>
 
int main()
{
    int num;
 
    printf("输入一个数字 : ");
    scanf("%d",&num);
 
    (num%2==0)?printf("偶数"):printf("奇数");
    //if num % 2 == 0, it will print 偶数, which is the result at left side.
    //if num % 2 == 1, it will print 奇数, which is the result at right side.
}
```





