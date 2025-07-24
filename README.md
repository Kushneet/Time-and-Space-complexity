# Time-and-Space-complexity
# 📈 Time and Space Complexity Cheatsheet

This guide covers core concepts like **Time Complexity**, **Space Complexity**, **Big O**, and their common types and hierarchies — perfect for interviews and coding contests.

---

## ✅ What is Time Complexity?

Time complexity is the amount of **time** taken by an algorithm to run, as a function of the input size **n**.  
It helps us understand how well an algorithm **scales** with larger inputs.

---

## ✅ Why Time Complexity?

- To **analyze algorithm efficiency**
- To **avoid Time Limit Exceeded (TLE)** errors in coding platforms
- To **compare algorithms** for large inputs (e.g., `n ≤ 10⁶`)

---

## 🔢 Notations

### 🟢 Big O Notation — `O()`

- Describes the **worst-case** scenario
- Upper bound on time

> Example: `O(n²)` means time increases quadratically with input

---

### 🟡 Theta Notation — `Θ()`

- Describes the **exact (tight bound)** behavior
- Both best and worst-case are the same

> Example: `Θ(n log n)`

---

### 🔴 Omega Notation — `Ω()`

- Describes the **best-case** scenario
- Lower bound

> Example: `Ω(n)` for an algorithm that runs faster on sorted data

---

## 🕓 Types of Time Complexities

| Complexity      | Name         | Example                        |
|----------------|--------------|--------------------------------|
| `O(1)`         | Constant      | Accessing array element        |
| `O(log n)`     | Logarithmic   | Binary Search                  |
| `O(n)`         | Linear        | Loop through array             |
| `O(n log n)`   | Linearithmic  | Merge Sort, Heap Sort          |
| `O(n²)`        | Quadratic     | Bubble Sort, Nested loops      |
| `O(n³)`        | Cubic         | 3 nested loops                 |
| `O(2ⁿ)`        | Exponential   | Recursive Fibonacci            |
| `O(n!)`        | Factorial     | Brute force permutations       |

---

## 📊 Complexity Hierarchy
O(1) < O(log n) < O(n) < O(n log n) < O(n²) < O(n³) < O(2ⁿ) < O(n!)


---

## 🧠 10⁸ Rule of Thumb (for CP & Interviews)

You can safely execute around **10⁸ operations per second**.

| Input Size `n`      | Max Acceptable Complexity |
|---------------------|---------------------------|
| `≤ 10`              | `O(n!)`, `O(2ⁿ)`          |
| `≤ 15–20`           | `O(2ⁿ)`                   |
| `≤ 100`             | `O(n³)`                   |
| `≤ 400`             | `O(n²)`                   |
| `≤ 2,000`           | `O(n²)`                   |
| `≤ 10⁴`             | `O(n log n)`              |
| `≤ 10⁶`             | `O(n)` or `O(n log n)`    |
| `≤ 10⁸`             | `O(1)` or `O(log n)`      |

---

## 💾 Space Complexity

Space complexity measures the amount of **extra memory** an algorithm uses (excluding input).

### Examples:

| Algorithm         | Space Complexity |
|------------------|------------------|
| Linear Search     | `O(1)`           |
| Merge Sort        | `O(n)`           |
| Quick Sort (in-place) | `O(log n)`    |
| Recursive DFS     | `O(n)`           |

---

## 📌 Bonus Tips

- Use `O(n log n)` or better for large `n`
- Watch out for recursive stack space
- Understand whether your code is CPU or memory-bound

---

> 📷 Based on notes from: **Lecture 11 – Time & Space Complexity** (Image Reference Included)

