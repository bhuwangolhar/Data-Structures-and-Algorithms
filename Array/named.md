# Arrays

## 📌 Definition

An **array** is a linear data structure used to store a fixed-size sequence of elements of the same data type.
In Java, arrays are objects that provide indexed access to elements, where indexing starts from `0`.

---

## ⚙️ Key Characteristics

* **Fixed Size**: Length is defined at the time of creation and cannot be changed.
* **Homogeneous Elements**: All elements must be of the same data type.
* **Contiguous Memory Allocation**: Elements are stored in consecutive memory locations.
* **Index-Based Access**: Enables fast retrieval using indices.
* **Zero-Based Indexing**: First element is at index `0`.
* **Direct Memory Access**: Enables constant time access (O(1)).
* **Object in Java**: Arrays are treated as objects and stored in heap memory.
* **Supports Multi-Dimensional Structures**: Can represent matrices and tables.

---

## 🧱 Declaration & Initialization

### 1. Declaration

```java
int[] arr;
```

### 2. Initialization

```java
arr = new int[5]; // creates array of size 5
```

### 3. Declaration + Initialization

```java
int[] arr = new int[5];
```

### 4. Direct Initialization

```java
int[] arr = {10, 20, 30, 40, 50};
```

### 5. Default Values

* `int` → 0
* `boolean` → false
* `object` → null

---

## 🔍 Accessing Elements

```java
int first = arr[0];   // first element
int third = arr[2];   // third element
```

* Access is **constant time O(1)** due to direct indexing.
* Accessing an invalid index results in `ArrayIndexOutOfBoundsException`.

---

## 🔁 Traversal

### Using for loop

```java
for (int i = 0; i < arr.length; i++) {
    System.out.println(arr[i]);
}
```

### Using enhanced for loop

```java
for (int num : arr) {
    System.out.println(num);
}
```

* Enhanced loop is cleaner but does not provide index control.

---

## 🔧 Common Operations

### 1. Insertion (at index)

```java
arr[2] = 25;
```

> Note: True insertion requires shifting elements → O(n)

---

### 2. Update

```java
arr[1] = 100;
```

---

### 3. Deletion

* Not directly supported.
* Typically handled by shifting elements manually.
* Leaves unused space at the end.

---

### 4. Searching

**Linear Search**

```java
for (int i = 0; i < arr.length; i++) {
    if (arr[i] == target) {
        // found
    }
}
```

> Binary search can be used if the array is sorted.

---

## 🔹 Types of Arrays in Java

### 1️⃣ One-Dimensional Array (1D)

A 1D array is a simple linear collection of elements.

```java
int[] arr = {1, 2, 3, 4, 5};
```

Access:

```java
System.out.println(arr[0]); // 1
```

---

### 2️⃣ Two-Dimensional Array (2D)

A 2D array is an array of arrays, often used to represent matrices.

```java
int[][] matrix = {
    {1, 2, 3},
    {4, 5, 6}
};
```

Access:

```java
System.out.println(matrix[1][2]); // 6
```

Traversal:

```java
for (int i = 0; i < matrix.length; i++) {
    for (int j = 0; j < matrix[i].length; j++) {
        System.out.print(matrix[i][j] + " ");
    }
}
```

---

###  ☂️ Jagged Arrays

Java allows arrays with different column sizes:

```java
int[][] jagged = {
    {1, 2},
    {3, 4, 5}
};
```

---

## ⏱️ Time Complexity (Basic Operations)

| Operation | Time Complexity |
| --------- | --------------- |
| Access    | O(1)            |
| Update    | O(1)            |
| Traversal | O(n)            |
| Search    | O(n)            |
| Insertion | O(n)            |
| Deletion  | O(n)            |

---

## 🚀 Space Complexity

| Structure | Space Complexity |
| --------- | ---------------- |
| 1D Array  | O(n)             |
| 2D Array  | O(n × m)         |

* Space depends on number of elements stored.
* No extra memory overhead (unlike dynamic structures like lists).
* In recursion problems involving arrays, additional stack space may be used.

---

## 🧠 Memory Representation

* Arrays are stored in **contiguous memory locations**.

* Each element is accessed using:

  `address = base_address + (index × size_of_element)`

* In 2D arrays (Java), memory is actually an array of references (not strictly contiguous like C).

---

## 🎯 Advantages

* Fast access using index (O(1))
* Simple and easy to use
* Memory efficient (no extra overhead)
* Cache-friendly due to contiguous storage
* Useful for implementing other data structures

---

## ⚠️ Limitations

* Fixed size (cannot grow dynamically)
* Insertion and deletion are costly
* Wastage of memory if size is overestimated
* Requires contiguous memory allocation
* Not suitable for frequent dynamic operations

---

## 📍 When to Use Arrays

* When the number of elements is known beforehand
* When fast access is required
* When working with simple, fixed datasets
* When memory efficiency is important
* When implementing low-level or performance-critical logic

---

## 📖 Summary

Arrays are one of the most fundamental and widely used data structures in Java. They provide **constant-time access**, simple syntax, and efficient memory usage, making them ideal for storing and processing fixed-size collections of data. They serve as the **foundation for advanced data structures** such as ArrayLists, stacks, queues, and matrices. While arrays are powerful due to their speed and simplicity, their limitations—such as fixed size and costly insertions/deletions—make them less suitable for highly dynamic scenarios. Understanding arrays deeply is essential, as many algorithmic problems and real-world applications rely on array-based logic and optimizations.

---
