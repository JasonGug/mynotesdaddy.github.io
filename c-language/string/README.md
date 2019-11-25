# String



Strings in C are actually arrays of characters. Although using pointers in C is an advanced subject, fully explained later on, we will use pointers to a character array to define simple strings, in the following manner:

{% hint style="danger" %}
There is no Type String in C.
{% endhint %}

```c
char * name = "John Smith";

char name[] = "John Smith";  
//Same as
char name[11] = "John Smith";

```

{% hint style="warning" %}
 The reason that we need to add one, although the string `John Smith` is exactly 10 characters long, is for the string termination: a special character `\0` \(equal to 0\) which indicates the end of the string. The end of the string is marked because the program does not know the length of the string - only the compiler knows it according to the code.
{% endhint %}

