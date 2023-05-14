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

## Literals

1. Integer Literals

   ```java
    int decimal = 10; // decimal value
    int octal = 07 // octal value and octal value must starts with 0, octal value range 0-7;
    int hex = 0xa12; // hexadecimal value starts with 0x, x is case in sensitive;
    int binary = 0b110101; // binary value starts with 0b, b is case in sensitive;
    int specialNum = 10_00_000; // _ has nothing in functional. it just easily separate digit groups;
   ```

2. Floating-Point Literals

   ```java
    float decimal = 10.0; // decimal value
    float octal = 07.6 // octal value and octal value must starts with 0, octal value range 0-7;
    float hex = 0xa12.03; // hexadecimal value starts with 0x, x is case in sensitive;
    float binary = 0b110101.011; // binary value starts with 0b, b is case in sensitive;
    float specialNum = 10_00_000.00; // _ has nothing in functional. it just easily separate digit groups;
   ```

3. Boolean Literals

    ```java
    boolean b = true; // either true or false only
    ```

4. Character Literals

    ```java
    char c = 'A'; //All of the visible ASCII characters can be directly entered inside the quotes, such as 'a', 'z', and '@
    char c1 = ''; //impossible to enter directly, there are several escape sequences that allow you to enter the character you need, such as '\'' for the single-quote character itself and '\n' for the newline character.
    char c2 = '/141'; // For octal notation, use the backslash followed by the three-digit number
    char c3 = '\ua432'; //. For hexadecimal, you enter a backslash-u ( \u), then exactly four hexadecimal digits
    ```

5. String Literals

    > String literals in Java are specified like they are in most other languages—by enclosing a sequence of characters between a pair of double quotes. Examples of string literals are

    ```java
    String str1 = "hello world"
    String str2 = "two\nthree"; // \n for new line
    ```

    | Escape Sequence | Description                                                  | Example             |
    | --------------- | ------------------------------------------------------------ | ------------------- |
    | \ddd            | Octal character (ddd)                                        | "\141"              |
    | \uxxxx          | Hexadecimal Unicode character (xxxx)                         | "\u1f6"             |
    | \'              | Single quote                                                 | "d\'nt"             |
    | \"              | Double quote                                                 | "\"this is quota\"" |
    | \\              | Backslash                                                    | "//"                |
    | \r              | Carriage return                                              |
    | \n              | New line (also known as line feed)                           |
    | \f              | Form feed                                                    |
    | \t              | Tab                                                          |
    | \b              | Backspace                                                    |
    | \s              | Space (added by JDK 15)                                      |
    | \endofline      | Continue line (applies only to text blocks; added by JDK 15) |
