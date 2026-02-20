# Java Practice Problems
## Increment / Decrement with Relational and Logical Operators

This document contains many practice problems using:

- Post-Increment (x++)
- Pre-Increment (++x)
- Post-Decrement (x--)
- Pre-Decrement (--x)
- Relational Operators
- Logical Operators

All answers are given at the end of the document.

Read each problem carefully and try to solve it before checking the answers.

---

# Section 1: Basic Increment and Decrement

### Problem 1
```java
int x = 5;
System.out.println(x++);
System.out.println(x);
```

---

### Problem 2
```java
int x = 5;
System.out.println(++x);
System.out.println(x);
```

---

### Problem 3
```java
int x = 5;
System.out.println(x--);
System.out.println(x);
```

---

### Problem 4
```java
int x = 5;
System.out.println(--x);
System.out.println(x);
```

---

# Section 2: Mixed Increment Expressions

### Problem 5
```java
int x = 5;
int y = x++ + ++x;
System.out.println(x);
System.out.println(y);
```

---

### Problem 6
```java
int a = 3;
int b = a++ + a++;
System.out.println(a);
System.out.println(b);
```

---

### Problem 7
```java
int a = 4;
int b = ++a + ++a;
System.out.println(a);
System.out.println(b);
```

---

# Section 3: Increment with Relational Operators

### Problem 8
```java
int x = 5;
System.out.println(x++ > 5);
System.out.println(x);
```

---

### Problem 9
```java
int x = 5;
System.out.println(++x > 5);
System.out.println(x);
```

---

### Problem 10
```java
int x = 5;
System.out.println(x-- >= 5);
System.out.println(x);
```

---

### Problem 11
```java
int x = 5;
System.out.println(--x >= 5);
System.out.println(x);
```

---

# Section 4: Logical AND (&&)

Logical AND returns true only if both conditions are true.

### Problem 12
```java
int x = 5;
System.out.println(x++ > 4 && x < 7);
System.out.println(x);
```

---

### Problem 13
```java
int x = 5;
System.out.println(++x > 6 && x++ < 10);
System.out.println(x);
```

---

### Problem 14
```java
int x = 5;
System.out.println(x++ > 10 && ++x < 20);
System.out.println(x);
```

---

# Section 5: Logical OR (||)

Logical OR returns true if at least one condition is true.

### Problem 15
```java
int x = 5;
System.out.println(x++ > 4 || x < 2);
System.out.println(x);
```

---

### Problem 16
```java
int x = 5;
System.out.println(++x > 6 || x++ < 10);
System.out.println(x);
```

---

### Problem 17
```java
int x = 5;
System.out.println(x++ > 10 || ++x < 20);
System.out.println(x);
```

---

# Section 6: Logical NOT (!)

### Problem 18
```java
int x = 5;
System.out.println(!(x++ > 4));
System.out.println(x);
```

---

# Important Concept: Short-Circuit

For &&:
If first condition is false, second condition will NOT execute.

For ||:
If first condition is true, second condition will NOT execute.

This affects increment and decrement operations.

---

# Answers Section

### Answer 1
5
6

### Answer 2
6
6

### Answer 3
5
4

### Answer 4
4
4

### Answer 5
7
12

### Answer 6
5
7

### Answer 7
6
11

### Answer 8
false
6

### Answer 9
true
6

### Answer 10
true
4

### Answer 11
false
4

### Answer 12
true
6

### Answer 13
false
6

### Answer 14
false
6

### Answer 15
true
6

### Answer 16
false
6

### Answer 17
true
7

### Answer 18
false
6

---


