# C Constant

## Constant

* Constant has a fixed value and it will not change throughout the whole process.
* Constant can be all types of variables.

## Escape Sequence \(转义序列\)

* In C, there are some special character. With the `\` in front, it has another meaning.
* [Escape Sequence Examples](../basic-c/escape-sequence-examples.md)

## Defining a constant in C

### Using `#define`

```c
#define LENGTH 10   
#define WIDTH  5
#define NEWLINE '\n'

int main()
{
    // ... code
}
```

### Using `const` 

```c
int main()
{
   const int  LENGTH = 10;
   const int  WIDTH  = 5;
   const char NEWLINE = '\n';
   
   // ... code
}
```

{% hint style="info" %}
It will be a good practice if we can keep constant all **Capitalized**. 
{% endhint %}



