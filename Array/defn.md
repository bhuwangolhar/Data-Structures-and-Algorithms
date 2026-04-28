# String Patterns & Techniques

## 📌 Introduction

Understanding strings is not just about storing and accessing characters—it involves recognizing **common patterns and techniques** used in string-based problem solving, where character-level manipulation and substring logic play a key role.

Mastering these patterns helps in writing efficient and optimized solutions.

---

## 🔁 Traversal Pattern

The most basic pattern used to process each character sequentially.

```java id="sp1"
for (int i = 0; i < str.length(); i++) {
    char ch = str.charAt(i);
}
```

### Use Cases

* Counting characters
* Printing or transforming strings
* Basic validations

---

## 🔄 Two Pointer Technique

Uses two indices to process the string from different directions.

```java id="sp2"
int left = 0;
int right = str.length() - 1;
```

### Variations

* Opposite direction (start & end)
* Same direction (slow & fast pointers)

### Use Cases

* Palindrome check
* Reversing a string
* Removing characters

---

## 🪟 Sliding Window Technique

Maintains a dynamic window over the string.

```java id="sp3"
int start = 0;

for (int end = 0; end < str.length(); end++) {
    // expand window

    while (condition) {
        start++;
    }
}
```

### Use Cases

* Longest substring problems
* Unique character tracking
* Window-based optimizations

---

## 🔍 Searching Techniques

### Linear Search

* Traverse character by character
* Works for any string

### Pattern Matching (Basic)

* Compare substrings
* Used in simple matching problems

---

## 🔃 Frequency Count Technique

Tracks occurrences of characters.

```java id="sp4"
int[] freq = new int[26];
```

### Use Cases

* Anagram detection
* Character counting
* Frequency comparison

---

## 🔁 In-Place vs New String Creation

### In-Place (using mutable structures)

```java id="sp5"
StringBuilder sb = new StringBuilder(str);
```

### New String Creation

```java id="sp6"
str = str + "a";
```

---

## ⚖️ Brute Force vs Optimized

### Brute Force

* Check all substrings
* Higher time complexity

### Optimized Approach

* Uses patterns like:

  * Sliding window
  * Two pointers
  * Frequency count

---

## ⚠️ Common Pattern Mistakes

* Ignoring empty or null strings
* Incorrect pointer updates
* Using inefficient substring operations
* Not identifying repeating patterns
* Off-by-one errors

---

## 📖 Summary

String problem solving is largely based on recognizing repeating patterns such as traversal, two pointers, sliding window, and frequency counting, and mastering these techniques allows developers to efficiently manipulate text data, reduce time complexity, and transition from brute force approaches to optimized solutions while improving overall problem-solving skills.

---
