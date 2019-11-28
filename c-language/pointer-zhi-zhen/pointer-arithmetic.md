# Pointer Arithmetic

### 16 bit Machine \(Turbo C\)

In a 16 bit machine, size of all types of pointer, be it `int*`, `float*`, `char*` or `double*` is always **2 bytes**. But when we perform any arithmetic function like increment on a pointer, changes occur as per the size of their primitive data type.

### **Size of datatypes on 16-bit Machine:**

| Type | Size \(in bytes\) |
| :--- | :--- |
| int or signed int | 2 |
| char | 1 |
| long | 4 |
| float | 4 |
| double | 8 |
| long double | 10 |

### Examples for Pointer Arithmetic

Now lets take a few examples and understand this more clearly.

```c
int* i;
i++;
```

In the above case, pointer will be of 2 bytes. And when we increment it, it will increment by 2 bytes because `int` is also of 2 bytes.

```c
float* i;
i++;
```

In this case, size of pointer is still 2 bytes initially. But now, when we increment it, it will increment by 4 bytes because `float` datatype is of 4 bytes.

```c
double* i;
i++;
```

Similarly, in this case, size of pointer is still 2 bytes. But now, when we increment it, it will increment by 8 bytes because its data type is `double`.

