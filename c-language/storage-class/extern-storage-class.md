# Extern Storage Class

Similar to Static Storage Class, extern storage class is to create a global variable as well. However, this variable is visible from all files.

{% tabs %}
{% tab title="main.c" %}
```c
#include <stdio.h>
 
int count ;
extern void write_extern();
 
int main()
{
   count = 5;
   write_extern();
}
```
{% endtab %}

{% tab title="support.c" %}
```c
#include <stdio.h>
 
extern int count;
 
void write_extern(void)
{
   printf("count is %d\n", count);
}
```
{% endtab %}
{% endtabs %}



