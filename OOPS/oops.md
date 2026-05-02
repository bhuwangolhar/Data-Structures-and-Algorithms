# Object

## 📌 Definition

An **object** is an instance of a class that represents a real-world entity with **state (data)** and **behavior (methods)**.
In Java, objects are created from classes and are used to access and manipulate the properties and actions defined within the class.

---

## ⚙️ Key Characteristics

* **Instance of Class**: Created using a class blueprint
* **State**: Represented by variables (fields/attributes)
* **Behavior**: Represented by methods (functions)
* **Identity**: Each object has a unique reference in memory
* **Stored in Heap Memory**: Objects are allocated dynamically
* **Access via Reference**: Objects are accessed using reference variables
* **Encapsulation Support**: Combines data and methods in a single unit
* **Independent Instances**: Each object maintains its own data

---

## 🧱 Object Creation

### 1. Using new Keyword

```java
ClassName obj = new ClassName();
```

---

### Example

```java
class Car {
    String model;
    int speed;
}

Car c1 = new Car();
```

---

## 🔍 Accessing Members

```java
c1.model = "Tesla";
c1.speed = 120;

System.out.println(c1.model);
```

* Accessed using **dot (.) operator**
* Allows reading and modifying object data

---

## 🔁 Object Reference Behavior

```java
Car c1 = new Car();
Car c2 = c1;
```

* Both references point to the **same object**
* Changes via one reference affect the other

---

## 🔄 Multiple Objects

```java
Car c1 = new Car();
Car c2 = new Car();
```

* Each object has its **own separate memory**
* Changes in one do not affect the other

---

## 🔧 Common Operations

### 1. Assign Values

```java
obj.field = value;
```

---

### 2. Call Methods

```java
obj.method();
```

---

### 3. Compare Objects

```java
obj1 == obj2; // compares reference
```

> Use `.equals()` for logical comparison (if overridden)

---

### 4. Passing Objects to Methods

```java
void update(Car c) {
    c.speed = 150;
}
```

* Changes affect the original object due to reference passing

---

## ⏱️ Time Complexity

| Operation        | Time Complexity |
| ---------------- | --------------- |
| Access field     | O(1)            |
| Call method      | O(1)            |
| Reference assign | O(1)            |

---

## 🚀 Space Complexity

* Depends on number of fields → **O(n)**
* Memory allocated dynamically in heap
* Additional overhead for object metadata

---

## 🧠 Memory Representation

* Object is stored in **heap memory**
* Reference variable is stored in **stack memory**
* Reference holds the memory address of the object
* Multiple references can point to the same object

---

## 🎯 Advantages

* Represents real-world entities effectively
* Enables modular and reusable code
* Supports object-oriented programming principles
* Improves code readability and organization
* Allows multiple instances with independent data

---

## ⚠️ Limitations

* Requires proper memory management
* Can increase complexity in large systems
* Improper reference handling may cause bugs
* Slight memory overhead compared to primitive types

---

## 📍 When to Use Objects

* When modeling real-world entities
* When grouping related data and behavior
* When implementing object-oriented programming concepts
* When designing scalable and maintainable systems

---

## 📖 Summary

Objects are the core building blocks of object-oriented programming in Java, enabling developers to represent real-world entities through a combination of data and behavior while maintaining identity through references in memory; by storing objects in heap memory and accessing them through references, Java allows flexible interaction, sharing, and modification of data across different parts of a program, making it essential to understand how objects are created, referenced, and passed in order to build modular, reusable, and scalable applications that effectively utilize key OOP principles such as encapsulation, inheritance, polymorphism, and abstraction.

---
