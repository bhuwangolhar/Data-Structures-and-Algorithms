# Arrays in Java

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

---

## 🔍 Accessing Elements

```java
int first = arr[0];   // first element
int third = arr[2];   // third element
```

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

---

## 🔧 Common Operations

### 1. Insertion (at index)

```java
arr[2] = 25;
```

### 2. Update

```java
arr[1] = 100;
```

### 3. Deletion

* Not directly supported.
* Typically handled by shifting elements manually.

### 4. Searching

**Linear Search**

```java
for (int i = 0; i < arr.length; i++) {
    if (arr[i] == target) {
        // found
    }
}
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

## 🧠 Memory Representation

* Arrays are stored in **contiguous memory locations**.
* Each element is accessed using:

  `address = base_address + (index × size_of_element)`

---

## 🎯 Advantages

* Fast access using index (O(1))
* Simple and easy to use
* Memory efficient (no extra overhead)

---

## ⚠️ Limitations

* Fixed size (cannot grow dynamically)
* Insertion and deletion are costly
* Wastage of memory if size is overestimated

---

## 📚 When to Use Arrays

* When the number of elements is known beforehand
* When fast access is required
* When working with simple, fixed datasets

---

## 🚀 Summary

Arrays are one of the most fundamental data structures in Java, providing efficient access and simple storage for fixed-size collections of elements. They form the foundation for more advanced data structures like lists, stacks, and queues.

---
