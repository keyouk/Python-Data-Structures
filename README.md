[[TOC]]

# 

# **Data Structures and Algorithms**

## **1 - Data Structures**

This will provide a quick reference on what data structures are and when to use them.

 

### **Array (List)**

Fastest and simplest data structure (aside from variables). Should be used

> <sub>* When a dataset has a known size.

> <sub>* When a dataset is small.

> <sub>* Memory is an issue, takes less memory than a Linked List.

### 
**Record (Tuple)**

Tuples are sets of data that are immutable. They are smaller and less dynamic than Python lists, however are much faster and take much less space.

### **Linked List**

A Linked List is when a index in a list will references the next index in the list. This is useful for sequences. Use a linked list when

> <sub>* You need constant time insertions and deletions from the list

> <sub>* You don't know the size of the array needed (so you don't have to redeclare)

> <sub>* You don't need random access to any elements

> <sub>* You want to insert elements in the middle of the list

### **Binary Tree**

### 
**Queues**

### 
**Stacks**

### 
**Heaps**

A heap is a tree where it's parent node is greater than any of it's child nodes. Use it when:

> <sub>* You need quick access to the largest or smallest values. 

> <sub>* Useful for Priority Queues, schedulers (Where the earliest time is desired.

> <sub>* Allows for In Place sorting.

  

### **Hash Table** (Dictionary)

Each index has a unique integer assigned to it. The idea of a hash is to convert that number into a readable number using an algorithm. Usually integer of string % length of array. Best used when:

> <sub>* Need O(1) time complexity. 

> <sub>* Each value in dataset is unique.

> <sub>* Store information in categories.

## **2. Searching and Sorting**

Sorting algorithms puts elements on a list in a certain order. This is used for easier access to data. This reference guide will provide references on when to use which types of sorts. As a note, anything with an O(N^2) complexity should not be used for large lists. 


References: [Here](http://python3.codes/popular-sorting-algorithms/)

### **Bubble Sort**

Very simple Algorithm. Algorithm starts at the beginning of the set, and if the next integer is bigger, it swaps them. This continues until the end of the list or when no swaps were made.

Use this when:

> <sub>* Use if List is short. 

> <sub>* Can also be used if elements are not extremely out of place.

Time Complexity: O(n^2)

Space Complexity: O(1)

### **Insertion Sort**

Insertion sort is an algorithm that moves elements one at a time into the correct position. The first element in the array is considered to be the sorted part. Essentially will check the array for exactly where to place the element instead of iterating over and over. 

Use this when:

> <sub>* Finishing off a different type of sort such as a quick sort or a merge sort.

> <sub>* Used in tandem with more sophisticated algorithms.

Note: **The insertion can be sped up by taking advantage of the already sorted part, and binary searching in it for the insertion point (or just after it if the new item is greater than any item in it)**.

Complexity: O(n^2)

Space Complexity: O(1)

### **Selection Sort**

Selection sort is an in-place comparison sort. It will find the smallest element in the array, and then switch it with the first element. It then finds the second smallest element in the array and swaps it with the second element. It continues to do this until the array is sorted. The main advantage is that is uses the least amount of data swaps than in any other algorithm. 

Use this when:

> <sub>* Swapping data is very expensive.

> <sub>* When writing is very slow compared to reading.	


Time Complexity: O(n^2)

Space Complexity: O(1)

### **Merge Sorts** (Efficient Sort)

Merge sort takes advantage of merging already sorted lists into a new sorted list. It splits the list by halving it until the groups have 1 element or no elements left. It then merges the groups back together so that their elements are in order.

Use this when:

> <sub>* Merging two sorted sets of data together.

> <sub>* Scales very well to large lists.

Complexity: O(n * log(n)) - O(n)

### **Heap Sorts** (Efficient Sort)

Heap sort turns the array into a binary heap structure which allows it to efficiently retrieve the minimal/maximal value. Removes from the heap and builds into a new sorted list until done.

Use this when:

> <sub>* Can only be used on an array-like data structure

> <sub>* Uses a data structure called a heap to efficiently do a selection sort.

Complexity: O(n* logn)

### **Quick Sorts** (Efficient Sort)

Quick Sort partitions an array using an element called a pivot. Anything smaller than the pivot goes before it and anything bigger goes after it. The sublists are then recursively sorted. One of the fastest sorting algorithms. It's worst case performance however is O(n^2). 

Some things to note:

> <sub>* Fastest Sorting method

> <sub>* Has a chance to be O(n^2) complexity if choosing a bad pivot.

> <sub>* Important to choose a good pivot point

Complexity: Could be O(n^2)

# **In Depth Data structures**

## Lists

### Enumerate

Enumerate(list) returns a tuple of a count and an argument.

### List Comprehension

List Comprehensions will build a list in the way a mathematician would. You can iterate through a list and add a function in front of it, and the output list will have the function apply to each stage of the list.

### Mapping

## Tuples

## Hash Tables

Hash tables are super complex. In this section of the documentation, we will go through the different methods of implementing a hash table, as well as hash table collision resolutions.

### Hash Table Collision

### Separate Chaining

### Linear Probing

Linear probing will search for the next available empty slot in the array to assign a hashKey. 

### Separate Chaining with List Head Cells

### Open Addressing

### Cuckoo Hashing

# **Libraries**

# **Data Science Programming**

## **1 - Data Visualization**

### Scatter Plots

### Line Charts

### Bar Charts

### Pie Charts

# Object Oriented Programming

Recursive - 

# Glossary

References:

http://www-inst.eecs.berkeley.edu/~cs61a/sp12/

### Mutable vs Immutable

Python sees all data as objects. A mutable object means that it can be changed, an immutable object or dataset means that it cannot be changed. 

### Time Complexity vs Space Complexity

Time Complexity

Having O(n) time complexity means having a program or algorithm scale in time with the length of the list. Having small data structures will be faster with O(n), however anything with big data needs to be run in O(1).  O(1) means constant time, and will take almost the same amount of time to retrieve the data no matter what the size of the list. This is useful for huge data sets.

Space Complexity

Space complexity uses the same notation. However means something slightly different. Having O(n) space means having dynamic space that scales with a larger list. Having o(1) space means having a limited amount of space, and must always use the same amount of space. 

Time Complexity vs space Complexity Cheatsheet: [here](http://bigocheatsheet.com/)

