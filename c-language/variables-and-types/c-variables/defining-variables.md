# Defining variables

## Define a variable \(Int & Floating Point Number\)

To define the variable `foo` and `bar`

```c
int foo;
int bar = 1;
float flu = 1.4;
```

{% hint style="info" %}
 The variable `foo` can be used, but since we did not initialize it, we don't know what's in it. The variable `bar` contains the number 1 and the variable `flu` contains the float 1.4
{% endhint %}

```c
int a = 0, b = 1, c = 2, d = 3, e = 4;
a = b - c + d * e
printf("%d" , a); /* will print 11 (1 - 2 + 3 * 4)*/
```

Example of a full program

```c
#include <stdio.h>

int main() {
  int a = 3;
  float b = 4.5;
  double c = 5.25;
  float sum;

  sum = a + b + c;

  printf("The sum of a, b, and c is %f.", sum);
  /*sum = 12.750000*/
  return 0;
}
```

