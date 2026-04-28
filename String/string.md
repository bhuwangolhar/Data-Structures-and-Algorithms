# String

## 📌 Definition

A **string** is a sequence of characters used to represent text.
In Java, strings are objects of the `String` class and are **immutable**, meaning their values cannot be changed after creation.

---

## ⚙️ Key Characteristics

* **Immutable**: Once created, the value cannot be modified
* **Stored in String Pool**: Optimized memory storage
* **Index-Based Access**: Characters can be accessed using indices
* **Zero-Based Indexing**: First character is at index `0`
* **Object Type**: Strings are objects, not primitive types
* **Supports Unicode**: Can store different character sets

---

## 🧱 Declaration & Initialization

### 1. Using String Literal

```java
String str = "hello";
```

---

### 2. Using new Keyword

```java
String str = new String("hello");
```

---

## 🔍 Accessing Characters

```java
char ch = str.charAt(0); // 'h'
```

---

## 🔁 Traversal

```java
for (int i = 0; i < str.length(); i++) {
    System.out.println(str.charAt(i));
}
```

---

## 🔧 Common Operations

### 1. Length

```java
str.length();
```

---

### 2. Concatenation

```java
String result = str + " world";
```

---

### 3. Comparison

```java
str.equals("hello"); // content comparison
```

---

### 4. Substring

```java
str.substring(0, 2);
```

---

## ⏱️ Time Complexity

| Operation     | Time Complexity |
| ------------- | --------------- |
| Access char   | O(1)            |
| Traversal     | O(n)            |
| Concatenation | O(n)            |
| Substring     | O(n)            |

---

## 🚀 Space Complexity

* Depends on number of characters → **O(n)**

---

## 🎯 Advantages

* Easy to use
* Rich built-in methods
* Safe due to immutability

---

## ⚠️ Limitations

* Immutable → extra memory usage
* Slower for frequent modifications

---

## 📍 When to Use Strings

* Handling text data
* Input/output operations
* Processing words and sentences

---

## 📖 Summary

Strings in Java are immutable objects used to store and manipulate text efficiently, and their built-in methods, combined with safe memory handling through immutability, make them one of the most essential data types for real-world applications and algorithmic problem solving.

---
