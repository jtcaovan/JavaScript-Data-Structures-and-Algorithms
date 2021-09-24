# JavaScript Data Structures and Algorithms

## Introduction

This repo is a personal collection of notes designed to act as a study guide for my interview preparation

## Resources


## Table of Contents

* Problem Solving Strategies
* Big O Notation
* Recursion
* Searching Algorithms
* Bubble Sort

---
### Problem Solving Strategies
1) Understand the problem
    * Can you restate the problem in your own words?
    * What are the inputs?
    * What are the outputs?
    * Can the outputs be determined from the inputs? Do you have enough information to solve the problem?
    * How should you label important pieces of data?
    
3) Explore examples
    * Start with simple examples
    * Progress to more complex examples
    * Explore empty inputs (or edge cases)
    * What about invalid inputs
   
4) Break it down
    * Explicitly write out the steps
   
6) Solve/Simplify
    * Solve simpler or parts of the problem
    
9) Look back and refactor
    * Check the result
    * Can you understand it?
    * Can you improve performance?
    * Ask for different approaches - how did other people solve it?

---

### Big O Notation
Big O Notation is the mtric we use to describe and compare the efficiency of algorithms.

*Time Complexity*

*Space Complexity*

| Common Big O Runtimes | Fastest to Slowest |
| ----------- | ----------- |
| O(log n) | Log time (ex. binary search) | 
| O(n) | Linear (ex. simple search) | 
| O(n * log n) | fast sorting algo (ex. quicksort) | 
| O(n^2) | slow sorting algo (ex. selection sort) | 
| O(n!) | Really slow n factorial (ex. Traveling Salesman) | 


---

### Core Data Structures, Algorithms, and Concepts

| Data Structures | Algorithms | Concepts |
| ----------- | ----------- | ----------- |
| Linked Lists | Breadth-First Search | Bit Manipulation |
| Trees, Tries and Graphs | Depth-First Search | Memory (Stack vs. Heap) |
| Stacks & Queues | Binary Search | Recursion |
| Heaps | Merge Sort | Dynamic Programming |
| Vectors / ArrayLists | Quick Sort | Big O Time & Space |
| Hash Tables |  | |


### Hash Tables

A hash table organizes data so you can quickly look up values for a given key.
> Note: In JavaScript, hash tables are called objects

|	Average |	Worst Case |
| ----------- | ----------- |
| space	| O(n)|	O(n) |
| insert	| O(1)|  O(n) |
| lookup	| O(1)|	O(n) |
| delete	| O(1)|	O(n) |

Strengths:
* Fast lookups. Lookups take O(1)O(1) time on average.
* Flexible keys. Most data types can be used for keys, as long as they're hashable.

Weaknesses:
* Slow worst-case lookups. Lookups take O(n)O(n) time in the worst case.
* Unordered. Keys aren't stored in a special order. If you're looking for the smallest key, the largest key, or all the keys in a range, you'll need to look through every key to find it.
* Single-directional lookups. While you can look up the value for a given key in O(1)O(1) time, looking up the keys for a given value requires looping through the whole dataset—O(n)O(n) time.
* Not cache-friendly. Many hash table implementations use linked lists, which don't put data next to each other in memory.
