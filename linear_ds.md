# Linear Data Structures & Programming Patterns

---

## 1. Linear Data Structures

Linear data structures store elements in a **sequential order**.
The differences are mainly about **memory layout**, **access cost**, and **update behavior**.

### 1.1 Array

* Contiguous memory
* O(1) random access
* Fixed-size or dynamic

**Variants**

* Static array
* Dynamic array (ArrayList, Vector)

**Key properties**

* Cache-friendly
* Expensive middle insert/delete

---

### 1.2 Linked List

* Non-contiguous memory
* Node-based structure

**Types**

* Singly linked list
* Doubly linked list
* Circular linked list

**Key properties**

* O(1) insert/delete if node is known
* O(n) access

---

### 1.3 Stack (LIFO)

* Last In, First Out

**Implementation**

* Array-based
* Linked list-based

**Use cases**

* Recursion simulation
* Backtracking
* Expression evaluation

---

### 1.4 Queue (FIFO)

* First In, First Out

**Variants**

* Simple queue
* Circular queue
* Deque (double-ended queue)

**Use cases**

* Scheduling
* Buffers
* Streaming pipelines

---

### 1.5 String

* Conceptually an array of characters
* Specialized operations

**Key aspects**

* Pattern matching
* Hashing
* Automata-based processing

---

## 2. Programming Patterns on Linear Structures

Patterns are **ways of thinking**, not just code templates.

---

## 2.1 Pointer Movement Patterns

Focus: **How indices move**

### Single Pointer

* Linear scan
* Counting, filtering

### Two Pointers

* Same direction (slow–fast)
* Opposite direction (left–right)

### Multiple Pointers

* k-way merge
* Multi-partition problems

**Core idea:** Controlled pointer evolution with invariants.

---

## 2.2 Sliding Window Patterns

Focus: **Contiguous subarrays or substrings**

### Fixed Window

* Constant size window
* Rolling computations

### Variable Window

* Constraint-based resizing
* Monotonic expansion/shrinking

**Core idea:** Window as a state machine.

---

## 2.3 Accumulation & Prefix Patterns

Focus: **Range-based reasoning**

### Prefix Sum

* Fast range queries
* Transforms subtraction into lookup

### Difference Array

* Efficient range updates

### Running Aggregates

* Max, min, sum, XOR

**Core idea:** Algebra over sequences.

---

## 2.4 Stack-Based Patterns

Focus: **Past decisions constrain future ones**

### Monotonic Stack

* Next greater/smaller element
* Histogram problems

### Simulation Stack

* Expression parsing
* Undo/redo systems

**Core idea:** Enforcing partial order.

---

## 2.5 Queue-Based Patterns

Focus: **Temporal order**

### BFS-style Linear Traversal

* Level-wise processing

### Monotonic Queue

* Sliding window max/min

**Core idea:** Preserving causality.

---

## 2.6 Hash-Assisted Linear Patterns

Focus: **Memory for speed**

### Frequency Map

* Counting
* Duplicate detection

### Prefix Hash

* Subarray equivalence

### Seen Sets

* Cycle detection
* Membership tests

**Core idea:** Trading space for time.

---

## 2.7 Rearrangement & In-Place Patterns

Focus: **Permutation and stability**

### Partitioning

* Dutch National Flag
* Stable vs unstable partition

### In-place Transformations

* Reverse
* Rotate
* Cyclic replacement

**Core idea:** Structure-preserving mutations.

---

## 2.8 Recursion on Linear Structures

Focus: **Inductive definitions**

### Structural Recursion

* Linked lists
* Strings

### Divide and Conquer

* Merge-based techniques

### Tail Recursion

* Stack optimization

**Core idea:** Self-similarity of linear data.

---

## 3. Cross-Cutting Concepts

These explain *why* patterns work.

* **Invariants**
* **Amortized analysis**
* **Memory locality**
* **Streaming constraints**
* **Automata theory (for strings)**

---

## 4. Natural Extensions

Linear patterns evolve into:

* Segment trees, Fenwick trees
* Heaps and priority queues
* Online algorithms
* String automata (KMP, Z, suffix structures)
* Hardware-aware algorithms (SIMD, cache models)

---
