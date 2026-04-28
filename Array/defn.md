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
* **Memory Efficient (Pooling)**: Reuses existing string literals to save memory

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

* Access is **O(1)** using index-based retrieval

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

> `==` compares references, not values

---

### 4. Substring

```java
str.substring(0, 2);
```

---

### 5. Case Conversion

```java
str.toLowerCase();
str.toUpperCase();
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
* Additional space may be used due to immutability during modifications

---

## 🎯 Advantages

* Easy to use
* Rich built-in methods
* Safe due to immutability
* Supports efficient memory usage via String Pool

---

## ⚠️ Limitations

* Immutable → creates new objects on modification
* Slower for frequent updates
* Higher memory usage in repeated concatenation

---

## 📍 When to Use Strings

* Handling text data
* Input/output operations
* Processing words and sentences
* Pattern matching and validation tasks

---

## 📖 Summary

Strings in Java are immutable objects designed for efficient and secure handling of textual data, and their behavior is influenced by concepts such as the string pool and object immutability, which help optimize memory usage while ensuring thread safety; although they provide a rich set of built-in methods for manipulation and comparison, developers must be mindful of performance implications—especially during repeated modifications—making it important to understand when to use strings directly and when to rely on alternatives like `StringBuilder` for better efficiency in real-world applications and algorithmic problem solving.

---
