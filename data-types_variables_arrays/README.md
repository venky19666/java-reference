# Data types Reference

## is Strong typed language?

>Yes. it don’t allow implicit conversions between unrelated types.

```java
int a=10;
a=10.5 // error: incompatible types: possible lossy conversion from double to int
```

### Strongly vs. weakly typed

>Weakly-typed languages make conversions between unrelated types implicitly; whereas, strongly-typed languages don’t allow implicit conversions between unrelated types.

```javascript
//simple javascript showing weak typed
var a=10;
a="str"
console.log(a) // output: str
```

### Statically vs.dynamically typed

>Statically-typed programming languages do type checking (i.e., the process of verifying and enforcing the constraints of types on values) at compile-time, whereas dynamically-typed languages do type checks at runtime.
>
> Statically-typed: C, C++, Java.
>
> Dynamically-typed: Perl, Ruby Python, PHP, JavaScript.

## Data types

1. Primitive data types - includes byte, short, int, long, float, double, boolean and char

    ```java
    int myNum = 5;               // Integer (whole number)
    float myFloatNum = 5.99f;    // Floating point number
    char myLetter = 'D';         // Character
    boolean myBool = true;       // Boolean
    String myText = "Hello";     // String
    ```

2. Non-primitive data types - such as String, Arrays and Classes
