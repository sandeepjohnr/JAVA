# Java Notes 

---

# 1. Float and Double in Java

In Java, whenever you write a decimal number like 2.6, Java automatically treats it as a double.

Example:

```java
float f1 = 2.6;   // Compile-time error
```

This gives an error because:

* 2.6 is considered a double by default.
* double uses 8 bytes of memory.
* float uses 4 bytes of memory.
* Java does not allow automatic conversion from a bigger type (double) to a smaller type (float) because data may be lost.

This type of conversion is called narrowing conversion, and Java requires it to be done manually.

Correct ways:

```java
double d1 = 2.6;       // Correct because 2.6 is double
float f2 = 2.6f;       // Correct (adding f tells Java this is float)
float f3 = (float)2.6; // Correct (explicit type casting)
```

When you add "f" at the end, Java understands that the number should be treated as float instead of double.

Important concept:

* All decimal numbers are double by default.
* To make them float, you must add "f" or "F".

---

# 2. Char Data Type

The char data type is used to store a single character.

Example:

```java
char c1 = 'x';
char c2 = '3';
```

Rules:

* Must contain only one character.
* Must be enclosed in single quotes (' ').

Java stores characters using Unicode. ASCII is a subset of Unicode.
Each character has a numeric value.

Example:

```java
System.out.println((int)'x');
```

This prints the Unicode value of 'x'.

Important difference:

```java
char c = "x";   // Error
```

Double quotes create a String.
Single quotes create a char.

String can hold multiple characters.
char can hold only one character.

---

# 3. Non-Primitive Data Types

Non-primitive types do not store actual values directly.
They store the reference (address) of the object in memory.

Classes are non-primitive types.

Example:

```java
class A {
}

A a1;            // reference variable (no object yet)
A a2 = new A();  // object created
```

Explanation:

* a1 is only a reference variable.
* new A() creates an object in heap memory.
* a2 stores the address of that object.

If you print the object reference:

```java
System.out.println(a2);
```

It prints the class name and hashcode because Java prints the reference information.

---

# 4. Types of Variables in Java

Java has three main types of variables based on where they are declared.

Java does not allow global variables outside a class.

This is not allowed:

```java
int k = 7;   // Outside class (Invalid)
```

Everything must be inside a class.

---

## 4.1 Instance Variable

Declared inside a class but outside methods.

Example:

```java
class E {
    int j = 2;  // instance variable
}
```

Characteristics:

* Belongs to an object.
* Each object has its own copy.
* Stored in heap memory.
* Gets default value if not initialized.

Example:

```java
class Student {
    int marks;
}
```

If you create an object and print marks without initializing, it prints 0 because default value for int is 0.

---

## 4.2 Static Variable

Declared using static keyword.

Example:

```java
class E {
    static int k = 3;
}
```

Characteristics:

* Belongs to the class, not the object.
* Only one copy exists.
* Shared by all objects.
* Created when class is loaded.
* Stored in method area.
* Gets default value automatically.
* Default value for non-primitive types is null.

Accessing static variable:

```java
System.out.println(E.k);
```

You should access static variables using the class name.

If you change static variable value in one place, it changes everywhere because there is only one copy.

---

## 4.3 Local Variable

Declared inside a method.

Example:

```java
class A {
    public static void main(String[] args) {
        int a = 10;
        System.out.println(a);
    }
}
```

Characteristics:

* Exists only inside that method.
* Stored in stack memory.
* Must be initialized before use.
* No default value.
* Local variables cannot be accessed outside their method.


Example of error:

```java
int x;
System.out.println(x);  // Compile-time error due to no initialization
```


# 5. Operators in Java

Operators are symbols used to perform operations on variables and values.

---

## 5.1 Arithmetic Operators

1. Addition (+)

```java
System.out.println(5 + 2);  // 7
```

2. Subtraction (-)

```java
System.out.println(5 - 2);  // 3
```

3. Multiplication (*)

```java
System.out.println(5 * 2);  // 10
```

4. Division (/)

```java
System.out.println(5 / 2);   // 2
System.out.println(5.0 / 2); // 2.5
```

If both numbers are integers, result is integer.
If at least one number is decimal, result is decimal.

5. Modulus (%)

```java
System.out.println(5 % 2);  // 1
```

Modulus gives remainder.

---

# 6. Increment Operators

There are two types:

## 6.1 Post-Increment (x++)

First uses the value, then increases it.

```java
int x = 5;
System.out.println(x++);  // prints 5
System.out.println(x);    // prints 6
```

Step-by-step:

* Print current value (5)
* Then increase it to 6

---

## 6.2 Pre-Increment (++x)

First increases the value, then uses it.

```java
int x = 5;
System.out.println(++x);  // prints 6
```

Step-by-step:

* Increase value to 6
* Then print 6

---

# 7. Important Concepts to Remember

1. Decimal numbers are double by default.
2. float requires f at the end.
3. char stores single character and uses single quotes.
4. String uses double quotes.
5. Java does not allow global variables outside class.
6. Static variables are shared.
7. Instance variables are separate per object.
8. Local variables must be initialized before use.
9. Division between integers removes decimal part.
10. Modulus operator gives remainder.

---


