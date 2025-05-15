# 📘 DSA from Scratch (Java Edition)

Welcome to the **DSA from Scratch** course using **Java**. This repository contains beginner-friendly notes and code examples to help you build a solid foundation in programming and data structures.

---

## 📌 Contents

1. [Primitive Data Types](#primitive-data-types)
2. [Lossy & Lossless Conversions](#type-conversions)
3. [Wrapper Classes, Autoboxing & Unboxing](#wrapper-classes-autoboxing--unboxing)
4. [Arrays](#arrays)
5. [Conditional Statements](#conditional-statements)
6. [Loops](#loops)
7. [Functions in Java](#functions-in-java)

---

## 🔢 Primitive Data Types

Java provides 8 built-in primitive types:

| Type      | Size    | Description                      | Example                |
| --------- | ------- | -------------------------------- | ---------------------- |
| `byte`    | 1 byte  | Small integers (-128 to 127)     | `byte a = 10;`         |
| `short`   | 2 bytes | Larger range of integers         | `short b = 200;`       |
| `int`     | 4 bytes | Default integer type             | `int c = 1000;`        |
| `long`    | 8 bytes | Very large integers              | `long d = 123456L;`    |
| `float`   | 4 bytes | Decimal numbers (low precision)  | `float e = 5.6f;`      |
| `double`  | 8 bytes | Decimal numbers (high precision) | `double f = 5.6;`      |
| `char`    | 2 bytes | Single characters                | `char g = 'A';`        |
| `boolean` | 1 bit   | `true` or `false` values         | `boolean flag = true;` |

---

## 🔁 Type Conversions

### ✅ Lossless Conversion (Widening)

Automatically converts smaller to larger types. No data is lost.

```java
int a = 10;
long b = a;  // int to long (lossless)
```

### ❌ Lossy Conversion (Narrowing)

Requires explicit casting. Data might be lost.

```java
long a = 100000L;
int b = (int) a;  // long to int (lossy)
```

---

## 📦 Wrapper Classes, Autoboxing & Unboxing

### 🔁 Autoboxing

Primitive → Wrapper Object

```java
int a = 5;
Integer obj = a; // autoboxing
```

### 🔄 Unboxing

Wrapper Object → Primitive

```java
Integer obj = 10;
int a = obj; // unboxing
```

### 📦 Common Wrapper Classes

| Primitive | Wrapper     |
| --------- | ----------- |
| `int`     | `Integer`   |
| `char`    | `Character` |
| `float`   | `Float`     |
| `double`  | `Double`    |
| `boolean` | `Boolean`   |
| `byte`    | `Byte`      |
| `short`   | `Short`     |
| `long`    | `Long`      |

---

## 📁 Arrays

Arrays are used to store multiple values of the same type in a single variable.

### Declaring and Initializing Arrays

```java
int[] numbers = new int[5]; // Declaration with size
numbers[0] = 10;
numbers[1] = 20;
```

### Array Literal

```java
int[] marks = {90, 85, 78, 92, 88};
```

### Accessing Elements

```java
System.out.println(marks[2]); // Output: 78
```

### Length of Array

```java
System.out.println(marks.length); // Output: 5
```

---

## ⏪ Conditional Statements

### `if` Statement

```java
int age = 18;
if (age >= 18) {
    System.out.println("Eligible to vote");
}
```

### `if-else` Statement

```java
int marks = 45;
if (marks >= 50) {
    System.out.println("Pass");
} else {
    System.out.println("Fail");
}
```

### `else-if` Ladder

```java
int marks = 85;
if (marks >= 90) {
    System.out.println("Grade A");
} else if (marks >= 75) {
    System.out.println("Grade B");
} else {
    System.out.println("Grade C");
}
```

### `switch` Statement

```java
int day = 3;
switch (day) {
    case 1: System.out.println("Monday"); break;
    case 2: System.out.println("Tuesday"); break;
    default: System.out.println("Other day");
}
```

---

## 🔁 Loops

### `for` Loop

```java
for (int i = 1; i <= 5; i++) {
    System.out.println(i);
}
```

### `while` Loop

```java
int i = 1;
while (i <= 5) {
    System.out.println(i);
    i++;
}
```

### `do-while` Loop

```java
int i = 1;
do {
    System.out.println(i);
    i++;
} while (i <= 5);
```

### `Enhanced For` Loop

Useful for iterating through arrays:

```java
int[] arr = {1, 2, 3, 4, 5};
for (int num : arr) {
    System.out.println(num);
}
```
### `for-each` Loop

```java
ArrayList<Integer> list = new ArrayList<>();
    list.add(10);
    list.add(20);
    list.add(30);

    list.forEach(num -> System.out.println(num));
```
---

## 🧠 Functions in Java

### Defining a Function

```java
public static void greet() {
    System.out.println("Hello, world!");
}
```

### Calling a Function

```java
public class Main {
    public static void main(String[] args) {
        greet();
    }
}
```

### Function with Parameters and Return

```java
public static int add(int a, int b) {
    return a + b;
}

public static void main(String[] args) {
    int result = add(5, 10);
    System.out.println("Sum: " + result);
}
```


---

## 🚀 Stay Connected

Feel free to ⭐ this repo and follow along as we build the full DSA course in Java. Contributions and feedback are welcome!
