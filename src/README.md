Assignment 3: Sorting and Searching Algorithm Analysis System
 Project Overview

This project implements and compares three fundamental algorithms:

Bubble Sort (basic sorting)
Quick Sort (advanced sorting)
Binary Search (searching)

The purpose of this experiment is to analyze their performance using execution time and understand how algorithm efficiency changes with input size and data structure.

 Algorithms Description
🔹 Bubble Sort

Bubble Sort is a simple comparison-based algorithm that repeatedly swaps adjacent elements if they are in the wrong order.

Time Complexity:
Worst: O(n²)
Best: O(n)
🔹 Quick Sort

Quick Sort is a divide-and-conquer algorithm that selects a pivot and partitions the array into smaller subarrays.

Time Complexity:
Average: O(n log n)
Worst: O(n²)
🔹 Binary Search

Binary Search works by repeatedly dividing a sorted array in half to locate a target value.

Time Complexity:
O(log n)
Requirement: array must be sorted
 Experimental Setup

The program tests algorithms using arrays of different sizes:

Small → 10 elements
Medium → 100 elements
Large → 1000 elements

For each size:

Random arrays are generated
Sorting algorithms are applied
Searching is performed on sorted arrays
Execution time is measured using System.nanoTime()
 Results (Example Output)
Array Size	Bubble Sort (ns)	Quick Sort (ns)	Binary Search (ns)
10	20000	5000	1000
100	500000	20000	2000
1000	5000000	100000	3000

(Actual results may vary depending on system performance)

 Analysis
Quick Sort is faster than Bubble Sort because it uses divide-and-conquer strategy and has better average complexity O(n log n).
Bubble Sort is slower, especially for large arrays, due to O(n²) complexity.
As array size increases, execution time increases significantly, especially for Bubble Sort.
Binary Search is very efficient with O(log n), much faster than linear approaches.
Binary Search requires a sorted array because it eliminates half of the data each step.
Screenshots


![1](../Docs/Screenshots/Output1.png)


Include:

Program output
Different test runs
 Reflection

This project helped me understand how algorithm efficiency affects performance in practice. I learned that theoretical complexity often matches real results, especially when working with large datasets.

One challenge was implementing Quick Sort correctly and ensuring Binary Search works only on sorted arrays. Overall, this assignment improved my understanding of sorting, searching, and performance measurement.

