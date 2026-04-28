# String (In-Depth)

## 📌 Introduction

Strings in Java involve important internal concepts such as **immutability, memory management, and string pooling**, which directly impact performance and behavior.

---

## ⚙️ String Pool

Java uses a special memory area called the **String Pool**.

```java
String a = "hello";
String b = "hello";
```

* Both refer to the same memory location

---

## 🔁 Immutability

```java
String str = "hello";
str = str + " world";
```

* Creates a new object instead of modifying the original

---

## 🔄 String vs StringBuilder vs StringBuffer

| Feature     | String | StringBuilder | StringBuffer |
| ----------- | ------ | ------------- | ------------ |
| Mutable     | No     | Yes           | Yes          |
| Thread Safe | No     | No            | Yes          |
| Performance | Slow   | Fast          | Medium       |

---

## 🧠 Why Immutability?

* Security
* Thread safety
* Caching (String Pool)

---

## 🔄 Common Operations Cost

```java
str = str + "a"; // creates new object
```

* Repeated concatenation → inefficient

---

## ⚠️ Common Mistakes

### 1. Using == instead of equals

```java
str1 == str2 // ❌
```

---

### 2. Frequent concatenation

```java
str = str + "a"; // ❌ in loops
```

---

### 3. Ignoring immutability

* Thinking string changes in-place

---

## 🧩 Real-World Usage

* Text processing
* Parsing input
* Pattern matching
* Data formatting

---

## ⏱️ Performance Considerations

* Use `StringBuilder` for modifications
* Avoid unnecessary string creation

---

## 📖 Summary

Strings in Java rely on immutability and memory optimization techniques such as the string pool, and understanding these internal behaviors helps developers write efficient, bug-free code while making better decisions between String, StringBuilder, and StringBuffer in performance-critical scenarios.

---
