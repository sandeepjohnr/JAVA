# Java Notes

---

# 1. Increment and Decrement Operators

Increment (++) increases value by 1.
Decrement (--) decreases value by 1.

There are two types:
1. Post-Increment (x++)
2. Pre-Increment (++x)

Similarly for decrement:
1. Post-Decrement (x--)
2. Pre-Decrement (--x)

---

# 2. Post-Increment (x++)

Rule:
First use the value, then increase it.

Example 1:

```java
int x = 5;
System.out.println(x++);
System.out.println(x);
```

Output:
```
5
6
```

Explanation:
Line 1 prints current value (5).
Then x becomes 6.

---

Example 2:

```java
int a = 10;
int b = a++;
System.out.println(a);
System.out.println(b);
```

Output:
```
11
10
```

Explanation:
b gets old value of a (10).
Then a becomes 11.

---

# 3. Pre-Increment (++x)

Rule:
First increase value, then use it.

Example 1:

```java
int x = 5;
System.out.println(++x);
```

Output:
```
6
```

---

Example 2:

```java
int a = 10;
int b = ++a;
System.out.println(a);
System.out.println(b);
```

Output:
```
11
11
```

Explanation:
First a becomes 11.
Then b gets 11.

---

# 4. Post-Decrement (x--)

Rule:
First use value, then decrease.

Example:

```java
int x = 5;
System.out.println(x--);
System.out.println(x);
```

Output:
```
5
4
```

---

# 5. Pre-Decrement (--x)

Rule:
First decrease, then use value.

Example:

```java
int x = 5;
System.out.println(--x);
```

Output:
```
4
```

---

# 6. Tricky Problems

Example 1:

```java
int x = 5;
int y = x++ + ++x;
System.out.println(x);
System.out.println(y);
```

Step-by-step:
Initial x = 5
x++ gives 5 (then x becomes 6)
++x makes x 7 and gives 7
So y = 5 + 7 = 12

Final Output:
```
7
12
```

---

Example 2:

```java
int a = 3;
int b = a++ + a++;
System.out.println(a);
System.out.println(b);
```

Step-by-step:
First a++ gives 3 (a becomes 4)
Second a++ gives 4 (a becomes 5)
b = 3 + 4 = 7

Output:
```
5
7
```

---

# 7. Relational Operators

Relational operators compare two values.
They always return boolean (true or false).

| Operator | Meaning |
|----------|----------|
| > | Greater than |
| < | Less than |
| >= | Greater than or equal |
| <= | Less than or equal |
| == | Equal to |
| != | Not equal to |

Example:

```java
System.out.println(5 > 3);   // true
System.out.println(5 < 3);   // false
System.out.println(5 == 5);  // true
System.out.println(5 != 2);  // true
```

Important:
== compares values for primitives.
For objects, it compares references.

---

# 8. Logical Operators

Logical operators work on boolean values.

| Operator | Meaning |
|----------|----------|
| && | Logical AND |
| || | Logical OR |
| ! | Logical NOT |

---

## 8.1 Logical AND (&&)

Returns true only if both conditions are true.

```java
System.out.println(true && true);   // true
System.out.println(true && false);  // false
System.out.println(5 > 3 && 10 > 2); // true
```

---

## 8.2 Logical OR (||)

Returns true if at least one condition is true.

```java
System.out.println(true || false);  // true
System.out.println(false || false); // false
```

---

## 8.3 Logical NOT (!)

Reverses the boolean value.

```java
System.out.println(!true);  // false
System.out.println(!false); // true
```

---

# 9. Difference Between Relational and Logical Operators

Relational operators compare values.
Logical operators combine boolean results.

Example:

```java
int x = 10;
System.out.println(x > 5 && x < 20);
```

First relational operators check conditions.
Then logical operator combines them.

---

# 10. Calling Static and Non-Static Methods

## 10.1 Static Method

Belongs to class.
Can be called using class name.

Example:

```java
class Demo {
    static void show() {
        System.out.println("Static method");
    }

    public static void main(String[] args) {
        Demo.show();
    }
}
```

No object required.

---

## 10.2 Non-Static Method (Instance Method)

Belongs to object.
Must create object to call it.

Example:

```java
class Demo {
    void display() {
        System.out.println("Non-static method");
    }

    public static void main(String[] args) {
        Demo d = new Demo();
        d.display();
    }
}
```

Object is required.

---

# 11. Important Rules

1. Static methods can directly access only static variables.
2. Static methods cannot directly access instance variables.
3. Instance methods can access both static and instance variables.
4. Static methods are called using class name.
5. Non-static methods are called using object reference.

---

# 12. Simple Summary

Post increment: Use then increase.
Pre increment: Increase then use.

Relational operators: Compare values.
Logical operators: Combine conditions.

Static method: Call using class name.
Non-static method: Call using object.

---



