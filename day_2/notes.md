# Day 2

## Methods Example

``` java
class Xyz {
    public static void main(String[] args) {
        System.out.println("start");
        Xyz.createOTP();
        System.out.println("end");
    }

    public static void createOTP() {
        System.out.println("OTP created");
    }
}
```

------------------------------------------------------------------------

## Method

A method is a set of statements used to perform a specific task.\
To execute the statements inside a method, calling the method is
compulsory.\
The `main` method is called by the JRE (Java Runtime Environment).

If we create a `public` class in a Java file, then the file name must be
the same as the class name.

We can create any number of default (non-public) classes in a Java file,
but we cannot create more than one `public` class in the same file.

------------------------------------------------------------------------

## Multiple Classes in One File

``` java
class X {
    public static void main(String[] args) {
        System.out.println("start");
        Y.createOTP();
        System.out.println("end");
    }
}

class Y {
    public static void createOTP() {
        System.out.println("OTP created");
    }
}
```

For the above code, both classes can be in the same file.\
When compiled, separate bytecode (`.class`) files will be generated for
each class.

------------------------------------------------------------------------

# Variables

A variable is a container used to store a value.

Java is a strictly typed programming language, which means a data type
must be specified while creating a variable.

### Syntax

``` java
dataType variableName;
variableName = value;
```

### Example

``` java
class Xyz {
    public static void main(String[] args) {
        int age; // declaration
        age = 23; // initialization
        System.out.println(age);
    }
}
```

------------------------------------------------------------------------

## Redeclaration of Variables

Redeclaration of a variable is not allowed in Java.

### Example (Error)

``` java
int n = 10;
System.out.println(n);
int n = 20; // Redeclaration - This will throw an error
System.out.println(n);
```

### Reinitialization (Allowed)

``` java
int n = 10;
System.out.println(n);
n = 20; // Reinitialization - This is allowed
System.out.println(n);
```

------------------------------------------------------------------------

# Data Types

There are two types of data types in Java:

## Primitive vs Non-Primitive

  Primitive   Non-Primitive
  ----------- -----------------
  byte        String
  short       class
  int         array
  long        object
  float       interface
  double      enum
  char        wrapper classes
  boolean     collections

------------------------------------------------------------------------

## Primitive Data Type Sizes

  Data Type   Size      Description
  ----------- --------- -----------------------------------------
  byte        1 byte    Stores small integers (-128 to 127)
  short       2 bytes   Stores medium integers
  int         4 bytes   Most commonly used integer type
  long        8 bytes   Stores very large integers
  float       4 bytes   Stores decimal numbers (less precision)
  double      8 bytes   Stores decimal numbers (high precision)
  char        2 bytes   Stores a single character (Unicode)
  boolean     1 bit\*   Stores true or false

\*Boolean size is JVM dependent internally but logically represents true
or false.
