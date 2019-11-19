# Variables and Types



C has several types of variables, but there are a few basic types

* **Integers** - whole numbers which can be either positive or negative. Defined using `char`, `int`, `short`, `long` or `long long`.
* **Unsigned integers** - whole numbers which can only be positive. Defined using `unsigned char`, `unsigned int`, `unsigned short`, `unsigned long` or `unsigned long long`
* **Floating point numbers** - real numbers \(numbers with fractions\). Defined using `float` and `double`.
* **Structures** - will be explained later, in the Structures section.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Variable Type</th>
      <th style="text-align:left">Size</th>
      <th style="text-align:left">Range</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">char</td>
      <td style="text-align:left">1 byte</td>
      <td style="text-align:left">
        <p>-128 - 127</p>
        <p>OR</p>
        <p>0 - 255</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">unsigned char</td>
      <td style="text-align:left">1 byte</td>
      <td style="text-align:left">0 - 255</td>
    </tr>
    <tr>
      <td style="text-align:left">signed char</td>
      <td style="text-align:left">1 byte</td>
      <td style="text-align:left">-128 - 127</td>
    </tr>
    <tr>
      <td style="text-align:left">int</td>
      <td style="text-align:left">
        <p>2 bytes</p>
        <p>OR</p>
        <p>4 bytes</p>
      </td>
      <td style="text-align:left">
        <p>-32,768 - 32767</p>
        <p>OR</p>
        <p>-2,147,483,648 - 2,147,483,647</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">unsigned int</td>
      <td style="text-align:left">
        <p>2 bytes</p>
        <p>OR</p>
        <p>4 bytes</p>
      </td>
      <td style="text-align:left">
        <p>0 - 65,535</p>
        <p>OR</p>
        <p>0 - 4,294,967,295</p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">short</td>
      <td style="text-align:left">2 bytes</td>
      <td style="text-align:left">-32,768 - 32,767</td>
    </tr>
    <tr>
      <td style="text-align:left">unsigned short</td>
      <td style="text-align:left">2 bytes</td>
      <td style="text-align:left">0 - 65,535</td>
    </tr>
    <tr>
      <td style="text-align:left">long</td>
      <td style="text-align:left">4 bytes</td>
      <td style="text-align:left">-2,147,483,648 - 2,147,483,647</td>
    </tr>
    <tr>
      <td style="text-align:left">unsigned long</td>
      <td style="text-align:left">4 bytes</td>
      <td style="text-align:left">0 - 4,294,967,295</td>
    </tr>
  </tbody>
</table>{% hint style="info" %}
Not that C does **not** have a Boolean type. Usually it is defined using the following notation.
{% endhint %}

```c
#define BOOL char
#define FALSE 0
#define TRUE 1
```

