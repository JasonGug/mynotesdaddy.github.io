# Two-dimensional Array

### Definition

In the previous tutorials on [Arrays](https://www.learn-c.org/en/Arrays), we covered, well, arrays and how they work. The arrays we looked at were all one-dimensional, but C can create and use multi-dimensional arrays. Here is the general form of a multidimensional array declaration.

![two-dimensional Array](../../.gitbook/assets/image%20%289%29.png)

```c
char characterAs[3][4] = {
    {'a', 'a', 'a', 'a'},
    {'a', 'a', 'a', 'a'},
    {'a', 'a', 'a', 'A'}
};

int val = characterAs[2][3]; //return A

```

