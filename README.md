<h1 align="center"> Data Structures and Algorithms in Java Basics </h1>

# Content

1. [Chapter 1: Introducing](#chapter1)
    - [Chapter 1 - Part 1: What is a Data Structure?](#chapter1part1)
    - [Chapter 1 - Part 2: What is an Algorithm?](#chapter1part2)
2. [Chapter 2: The Big-O Notation](#chapter2)
    - [Chapter 2 - Part 1: The Big-O Notation](#chapter2part1)

## <a name="chapter1"></a>Chapter 1: Introducing
  
#### <a name="chapter1part1"></a>Chapter 1 - Part 1: What is a Data Structure?

- Organizes and stores data
- Each has strenghts and weaknesses

A data structure is not only used for organizing the data. It is also used for processing, retrieving, and storing data. 
There are different basic and advanced types of data structures that are used in almost every program or software system that has been developed. So we must have good knowledge about data structures.

There are many types of data structures and the way that each stores and organizes data will differ. Ex: Arrays order the data sequentially and place each value in its own slot and we can get this slot using the index. A Tree is a hierarchical data structure.

Each data structure do somethings well and others not so well. Ex: A array is great for random access when you know the index of the item you wanna access but when you don't now the index, they are not so well because you have to search(loop) the dataset. 

<br>

<div align="center"><img src="img/typesofdatastructure-w660-h347.jpg" width=660 height=347><br><sub>Classification of Data Structure - (<a href='https://www.geeksforgeeks.org/data-structures/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- **Linear data structure**: Data structure in which data elements are arranged sequentially or linearly, where each element is attached to its previous and next adjacent elements, is called a linear data structure. 
Examples of linear data structures are array, stack, queue, linked list, etc.
  - **Static data structure**: Static data structure has a fixed memory size. It is easier to access the elements in a static data structure. 
An example of this data structure is an array.
  - **Dynamic data structure**: In dynamic data structure, the size is not fixed. It can be randomly updated during the runtime which may be considered efficient concerning the memory (space) complexity of the code. 
Examples of this data structure are queue, stack, etc.

- **Non-linear data structure**: Data structures where data elements are not placed sequentially or linearly are called non-linear data structures. In a non-linear data structure, we can’t traverse all the elements in a single run only. 
Examples of non-linear data structures are trees and graphs.

#### <a name="chapter1part2"></a>Chapter 1 - Part 1: What is an Algorithm?

An algorithm describes the steps you have to perform to accomplish a specific task.

Example of Making a Tea

1- Boil Water
2- Add a teabag to a cup
3- Pour the boiling water into the cup
4- Remove the teabag when tea is ready
5- Add the desired amount of milk to the cup
6- Add the desired amount of sugar to the cup
7- Stir the contents of the cup with a spoon

In this example, this is one algorithm to make a Tea. There is many ways to make tea, in this case, not just one algorithm to do the same thing.

For example, there many types of sort algorithm to sort data.

- There can be many algorithms that accomplish the same task
- There can be  many implementations of the same algorithm

**Types of Algorithms**

- Brute Force Algorithm
  - It is the simplest approach to a problem. A brute force algorithm is the first approach that comes to finding when we see a problem.

- Recursive Algorithm
  - A recursive algorithm is based on recursion. In this case, a problem is broken into several sub-parts and called the same function again and again.

- Backtracking Algorithm
  - The backtracking algorithm builds the solution by searching among all possible solutions. Using this algorithm, we keep on building the solution following criteria. Whenever a solution fails we trace back to the failure point build on the next solution and continue this process till we find the solution or all possible solutions are looked after.
 
- Searching Algorithm
  - Searching algorithms are the ones that are used for searching elements or groups of elements from a particular data structure. They can be of different types based on their approach or the data structure in which the element should be found.
 
- Sorting Algorithm
  - Sorting is arranging a group of data in a particular manner according to the requirement. The algorithms which help in performing this function are called sorting algorithms. Generally sorting algorithms are used to sort groups of data in an increasing or decreasing manner.
 
- Hashing Algorithm
  - Hashing algorithms work similarly to the searching algorithm. But they contain an index with a key ID. In hashing, a key is assigned to specific data.
 
- Divide and Conquer Algorithm
  - This algorithm breaks a problem into sub-problems, solves a single sub-problem, and merges the solutions to get the final solution. It consists of the following three steps:
    - Divide
    - Solve
    - Combine
   
- Greedy Algorithm
  - In this type of algorithm, the solution is built part by part. The solution for the next part is built based on the immediate benefit of the next part. The one solution that gives the most benefit will be chosen as the solution for the next part.
 
- Dynamic Programming Algorithm
  - This algorithm uses the concept of using the already found solution to avoid repetitive calculation of the same part of the problem. It divides the problem into smaller overlapping subproblems and solves them.
 
- Randomized Algorithm
  - In the randomized algorithm, we use a random number so it gives immediate benefit. The random number helps in deciding the expected outcome.
 
**How to Design an Algorithm?**

1- The problem that is to be solved by this algorithm i.e. clear problem definition.
2- The constraints of the problem must be considered while solving the problem.
3- The input to be taken to solve the problem.
4- The output is to be expected when the problem is solved.
5- The solution to this problem is within the given constraints.

Then the algorithm is written with the help of the above parameters such that it solves the problem.

## <a name="chapter2"></a>Chapter 2: The Big-O Notation
  
#### <a name="chapter2part1"></a>Chapter 2 - Part 1: The Big-O Notation

