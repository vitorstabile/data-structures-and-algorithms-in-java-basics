<h1 align="center"> Data Structures and Algorithms in Java Basics </h1>

# Content

1. [Chapter 1: Introducing](#chapter1)
    - [Chapter 1 - Part 1: What is a Data Structure?](#chapter1part1)
    - [Chapter 1 - Part 2: What is an Algorithm?](#chapter1part2)
2. [Chapter 2: The Big-O Notation](#chapter2)
    - [Chapter 2 - Part 1: The Big-O Notation](#chapter2part1)
3. [Chapter 3: Arrays in Java](#chapter3)
    - [Chapter 3 - Part 1: Quick Review of Arrays in Java](#chapter3part1)
    - [Chapter 3 - Part 2: Arrays in Memory](#chapter3part2)
    - [Chapter 3 - Part 3: Big-O Values for Array Operations](#chapter3part3)
    - [Chapter 3 - Part 4: Bubble Sort](#chapter3part4)
    - [Chapter 3 - Part 5: Stable vs Unstable Sort Algorithms](#chapter3part5)
    - [Chapter 3 - Part 6: Selection Sort](#chapter3part6)
    - [Chapter 3 - Part 7: Insertion Sort](#chapter3part7)
    - [Chapter 3 - Part 8: Shell Sort](#chapter3part8)
    - [Chapter 3 - Part 9: Recursion](#chapter3part9)
    - [Chapter 3 - Part 10: Merge Sort](#chapter3part10)
    - [Chapter 3 - Part 11: Quick Sort](#chapter3part11)
    - [Chapter 3 - Part 12: Counting Sort](#chapter3part12)
    - [Chapter 3 - Part 13: Radix Sort](#chapter3part13)
    - [Chapter 3 - Part 14: Sorting Arrays using JDK](#chapter3part14)
4. [Chapter 4: Lists in Java](#chapter4)
    - [Chapter 4 - Part 1: Introduction to Lists](#chapter4part1)
    - [Chapter 4 - Part 2: Array Lists](#chapter4part2)
    - [Chapter 4 - Part 3: Vectors](#chapter4part3)
    - [Chapter 4 - Part 4: Singly Linked Lists](#chapter4part4)
    - [Chapter 4 - Part 5: Doubly Linked Lists](#chapter4part5)
    - [Chapter 4 - Part 6: JDK LinkedList Class](#chapter4part6)
5. [Chapter 5: Stacks in Java](#chapter5)
    - [Chapter 5 - Part 1: Introduction to Stacks](#chapter5part1)
6. [Chapter 6: Queues in Java](#chapter6)
    - [Chapter 6 - Part 1: Introduction to Queues](#chapter6part1)
7. [Chapter 7: Hashtables in Java](#chapter7)
    - [Chapter 7 - Part 1: Introduction to Hashtables](#chapter7part1)
8. [Chapter 8: Search Algorithms](#chapter8)
    - [Chapter 8 - Part 1: Introduction to Search Algorithms](#chapter8part1)
9. [Chapter 9: Trees in Java](#chapter9)
    - [Chapter 9 - Part 1: Introduction to Trees](#chapter9part1)
10. [Chapter 10: Heaps in Java](#chapter10)
    - [Chapter 10 - Part 1: Introduction to Heaps](#chapter10part1)
11. [Chapter 11: Sets in Java](#chapter11)
    - [Chapter 11 - Part 1: Introduction to Sets](#chapter11part1)

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

#### <a name="chapter1part2"></a>Chapter 1 - Part 2: What is an Algorithm?

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

How can we be able to compare the performance of one algorithm against another algorithm? One way we could do that is to implement one algorithm and then put a line of code that records the start time and then run the implementation
and then have a line of code that records the end time and we can subtract the start time from the end time and we get the running time of the implementation of that algorithm. And then we do the same for another algorithm and we just compare the two.

In theory but unfortunately that's not a good way to do it because of hardware. Hardware is going to influence the running time of these algorithms. If we were to run an implementation on a desktop computer that was built in 2017 and compare that
to the running time of the exact same implementation on a desktop computer that was built 20 years ago and perhaps is an old Pentium computer, or we'll even go further than that and run the implementation on a Commodore 64 or something like that,
obviously the implementations are going to run slower on the older hardware. And if we were to run an implementation on a super computer, it's going to run really, really fast even though it might be a really inefficient algorithm.

So we need a more objective measure than just the straight running time. And so what we do is we look at the number of steps that it takes to execute an algorithm.

And we call this the **time complexity**.

There are two types of complexity:
  - **Time complexity**: which is the number of steps involved to run an algorithm.
  - **Memory complexity**: which is the amount of memory it takes to run an algorithm.

So we're interested in how many steps does it take to run an algorithm?

Now when we're doing we like to look at the worst case.

Looking at the best case doesn't help us because you're rarely gonna have the best case.

So if we wanna know what the upper bound is, like what is the absolute worst that we can expect from this algorithm, it's much more helpful to look at the worst case.

So it's helpful to compare the worst case scenario for one algorithm against the worst case scenario for the other algorithm.

We've already looked at an algorithm for making tea so now we're going to look at one little step.

```
1. Fetch the bowl containing the sugar
2. Get a Spoon
3. Scoop out sugar using the spoon
4. Pour the sugar from the spoon into the tea
5. Repeat steps 3 and 4 until you've added the desired amount of sugar
```

Now we can see from this that the number of steps that it's going to take to add sugar to your tea is going to depend on how many sugars you want.

If you only want one sugar, then this algorithm will run taking four steps. (1x1,2x1,3x1 and 4x1)

But if you want two sugars, it's going to take six steps because you're going to have to repeat steps three and four. (1x1,2x1,3x2 and 4x2)

So as we can see the number of steps or the time complexity of our sugar algorithm depends on how many sugars someone wants in their tea.

| Number of Sugars  | Steps Required  | 
| :---------------- | :--------------:|
| 1                 | 4               |
| 2                 | 6               |
| 3                 | 8               |
| 4                 | 10              |

If they only want one sugar, it just takes them four steps.

But if they want four sugars, it's gonna take them 10 steps.

So the time complexity gives us an idea of how an algorithm will perform as the number of items it has to deal with grows so as we can see as the number of sugars this algorithm has to add to tea increases, the number of steps required increases.

Another way of saying this is it tells us how well an algorithm will scale.

So how well will it do when it has to deal with 100 items, versus 1,00 items, versus a million items?

And we'll see that some algorithm will scale really well and others not so well.

The more items there are, the more algorithm's performance will degrade.

Now the big O notation is a way of expressing the complexity related to the number of items that an algorithm has to deal with. And it's written as a capital O followed by an expression in parenthesis.

So let's work out the big O value for our sugar algorithm.

- Number of desired sugars = n
- Total number of steps = 2n + 2
- As n grows, the number of steps grows
- The "2" in 2n and the "+2" reamin constant, so they don't factor into the time complexity. The value of n determines the growth rate
- Time complexity is O(n)
- Linear time complexity

| Big-O       |                 | 
| :---------- | :--------------:|
| O(1)        | Constant        |
| O(logn)     | Logarithmic     |
| O(n)        | Linear          |
| O(n.logn)   | n-log-star-n    |
| O(n^2)      | Quadratic       |



And so this is a graph of some of the big O values, and this represents how an algorithm would degrade.

Along the X axis we have the input size, so the number of items; and along the Y axis we have the number of steps.

<br>

<div align="center"><img src="img/bigographic-w1024-h1024.png" width=1024 height=1024><br><sub>Graphs of functions commonly used in the analysis of algorithms, showing the number of operations N versus input size n for each function - (<a href='https://en.wikipedia.org/wiki/Big_O_notation#/media/File:Comparison_computational_complexity.svg'>Work by Cmglee</a>) </sub></div>

<br>

Examples of each time complexity

- **O(1)**: Constant Time Execution

```java
int getFirst(int[] array) {
    return array[0];
}
```

In this case, we are returning the first element of the array, no matter the size of the array, the time to execute this function will always be the same.

- **O(logn)**: Logarithmic Time Execution

```java
boolean binarySearch(int[] array, int x) {
    int left = 0, right = array.length - 1;
    while (left <= right) {
        int mid = left + (right - left) / 2;
        if (array[mid] == x) {
            return true;
        }
        if (array[mid] < x) {
            left = mid + 1;
        } else {
            right = mid - 1;
        }
    }
    return false;
}
```

This is an example of binary search. At each step, we eliminate half of the elements. Therefore, the runtime increases logarithmically with the size of the array.

- **O(n)**: Linear Time Execution

```java
boolean contains(int[] array, int element) {
    for (int i = 0; i < array.length; i++) {
        if (array[i] == element) {
            return true;
        }
    }
    return false;
}
```

In this case, in the worst scenario, we have to traverse the whole array to find out if an element is present or not. Therefore, the execution time increases linearly with the size of the array.

- **O(n.logn)**: Linearithmic Time Execution

```java
class MergeSort { 
    // Merges two subarrays of arr[]. 
    // First subarray is arr[l..m] 
    // Second subarray is arr[m+1..r] 
    void merge(int arr[], int l, int m, int r) 
    { 
        // Find sizes of two subarrays to be merged 
        int n1 = m - l + 1; 
        int n2 = r - m; 
  
        // Create temp arrays 
        int L[] = new int[n1]; 
        int R[] = new int[n2]; 
  
        // Copy data to temp arrays 
        for (int i = 0; i < n1; ++i) 
            L[i] = arr[l + i]; 
        for (int j = 0; j < n2; ++j) 
            R[j] = arr[m + 1 + j]; 
  
        // Merge the temp arrays 
        // Initial indexes of first and second subarrays 
        int i = 0, j = 0; 
  
        // Initial index of merged subarray array 
        int k = l; 
        while (i < n1 && j < n2) { 
            if (L[i] <= R[j]) { 
                arr[k] = L[i]; 
                i++; 
            } 
            else { 
                arr[k] = R[j]; 
                j++; 
            } 
            k++; 
        } 
  
        // Copy remaining elements of L[] if any 
        while (i < n1) { 
            arr[k] = L[i]; 
            i++; 
            k++; 
        } 
  
        // Copy remaining elements of R[] if any 
        while (j < n2) { 
            arr[k] = R[j]; 
            j++; 
            k++; 
        } 
    } 
  
    // Main function that sorts arr[l..r] using 
    // merge() 
    void sort(int arr[], int l, int r) 
    { 
        if (l < r) { 
            // Find the middle point 
            int m = (l + r) / 2; 
  
            // Sort first and second halves 
            sort(arr, l, m); 
            sort(arr, m + 1, r); 
  
            // Merge the sorted halves 
            merge(arr, l, m, r); 
        } 
    } 
  
    // A utility function to print array of size n 
    static void printArray(int arr[]) 
    { 
        int n = arr.length; 
        for (int i = 0; i < n; ++i) 
            System.out.print(arr[i] + " "); 
        System.out.println(); 
    } 
  
    // Driver method 
    public static void main(String args[]) 
    { 
        int arr[] = { 12, 11, 13, 5, 6, 7 }; 
  
        System.out.println("Given Array"); 
        printArray(arr); 
  
        // Calling of Merge Sort 
        MergeSort ob = new MergeSort(); 
        ob.sort(arr, 0, arr.length - 1); 
  
        System.out.println("\nSorted array"); 
        printArray(arr); 
    } 
}

```

Merge Sort is a divide-and-conquer algorithm. It divides the input array into two halves, calls itself the two halves, and then merges the two sorted halves. The merge() function is used for merging two halves. The merge(arr, l, m, r) is a key process that assumes that arr[l..m] and arr[m+1..r] are sorted and merges the two sorted sub-arrays into one. 

Step 1 : Divide Array into Two Parts
Step 2: Merge Sort the first part of the array
Step 3: Merge Sort the second part of the array
Step 4: Merge Both the parts
Step 5: Return the Sorted Array

- **O(n^2)**: Quadratic Time Execution

```java
void printPairs(int[] array) {
    for (int i = 0; i < array.length; i++) {
        for (int j = 0; j < array.length; j++) {
            System.out.println(array[i] + ", " + array[j]);
        }
    }
}
```

In this case, for each element in the array, we are traversing the whole array again. This gives us a runtime that is the square of the size of the array.

- **O(2^n)**: Exponential Time Execution

```java
int fibonacci(int n) {
    if (n <= 1) {
       return n;
    }
    return fibonacci(n-1) + fibonacci(n-2);
}
```

This is an example of computing Fibonacci using recursion. For each number, we compute the two previous numbers, leading to an exponential runtime complexity.

- **O(n!)**: Fatorial Time Execution
```java
public class FactorialExample {

    public static void main(String[] args) {
        int[] array = {1, 2, 3}; // Sample array

        // Nested loops with O(n!) time complexity
        for (int i = 0; i < array.length; i++) {
            for (int j = 0; j < array.length; j++) {
                for (int k = 0; k < array.length; k++) {
                    System.out.println(array[i] + ", " + array[j] + ", " + array[k]);
                }
            }
        }
    }
}
```

In this example, the nested loops iterate over the array elements, printing out all possible combinations of three elements from the array. This results in a time complexity of O(n!), where n is the number of elements in the array.

## <a name="chapter3"></a>Chapter 3: Arrays in Java
  
#### <a name="chapter3part1"></a>Chapter 3 - Part 1: Quick Review of Arrays in Java

How to create and access elements in a array?

```java
public class Main {

    public static void main(String[] args) {
	    int[] intArray = new int[7];

	    intArray[0] = 20;
	    intArray[1] = 35;
	    intArray[2] = -15;
	    intArray[3] = 7;
	    intArray[4] = 55;
	    intArray[5] = 1;
	    intArray[6] = -22;

	    for (int i = 0; i < intArray.length; i++) {
	        System.out.println(intArray[i]);
        }
    }
}
```

We create a array with 7 slots with the index go from 0 to 6.

#### <a name="chapter3part2"></a>Chapter 3 - Part 2: Arrays in Memory

Arrays is:

- Contiguous block in memory
- Every element occupies the same amount of space in memory
- If a array starts at memory address x, and the size of each element in the array is y, we can calculate the memory address of the ith element by using the following expression: x + i*y
- If we know the index of an element, the time to retrieve the element will be the same, no matter where it is in the array.

For the array above of int

```
intArray[0] = 20;
intArray[1] = 35;
intArray[2] = -15;
intArray[3] = 7;
intArray[4] = 55;
intArray[5] = 1;
intArray[6] = -22;
````

Start address of array = 12, element size = 4 bytes

```
Address of array[0] = 12
Address of array[1] = 12 + (1*4) = 16
Address of array[2] = 12 + (2*4) = 20
Address of array[3] = 12 + (3*4) = 24
Address of array[4] = 12 + (4*4) = 28
Address of array[5] = 12 + (5*4) = 32
Address of array[6] = 12 + (6*4) = 36
```

This is because we begin with the index 0.

Now this is why a array is so efficient to retrieve a element when you now the index of this element. This is because doesn't matter where the element is in the array, we do the same calculation to retrieve them (x + i*y).

#### <a name="chapter3part3"></a>Chapter 3 - Part 3: Big-O Values for Array Operations

**Retrieve an Element from an Array**
- Multiply the size of the element by its index
- Get the start address of the array
- Add the start address to the result of the multiplication

For an int array, assume element starts at address 12. Each int is 4 bytes.

```
Address of array[0] = 12 + (0*4) = 12
Address of array[1] = 12 + (1*4) = 16
Address of array[2] = 12 + (2*4) = 20
Address of array[3] = 12 + (3*4) = 24
```

Doesn't matter how many elements we have, the number of the steps will be the same.

| Number of Elements | Steps to retrieve  | 
| :----------------- | :-----------------:|
| 1                  | 3                  |
| 1000               | 3                  |
| 100000             | 3                  |
| 1000000            | 3                  |
| 1000000000         | 3                  |

Now, let's see some operations in array and the time complexity

| Operation                                        | Time Complexity        | 
| :----------------------------------------------- | :---------------------:|
| Retrieve with index                              | O(1) - Constant time   |
| Retrieve without index                           | O(n) - Linear Time     |
| Add an element to a full array                   | O(n)                   |
| Add an element to the end of a array (has space) | O(1)                   |
| Insert or update an element ar a specific index  | O(1)                   |
| Delete an element by setting it to null          | O(1)                   |
| Delete an element by shifting element            | O(n)                   |

In resume, every time there is a For loop, will be a O(n) complexity

**Retrieve with index**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        int[] intArray = new int[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] = 55;
        intArray[5] = 1;
        intArray[6] = -22;

        System.out.println(intArray[3]);
    }
}
```

**Retrieve without index**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        int[] intArray = new int[7];

	    intArray[0] = 20;
	    intArray[1] = 35;
	    intArray[2] = -15;
	    intArray[3] = 7;
	    intArray[4] =55;
	    intArray[5] = 1;
	    intArray[6] = -22;

	    int index = -1;
	    for (int i = 0; i < intArray.length; i++) {
	        if (intArray[i] == 7) {
	            index = i;
	            break;
            }
        }

        System.out.println("index = " + index);
    }
}
```

**Add an element to a full array**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        int[] intArray = new int[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] =55;
        intArray[5] = 1;
        intArray[6] = -22;

        int newElement = 30;
        int[] intNewArray = new int[8];

        for (int i = 0; i < intArray.length; i++) {
            intNewArray[i] = intArray[i];
        }
        intNewArray[7] = newElement;

        System.out.println(Arrays.toString(intNewArray));
    }
}
```
**Add an element to the end of a array (has space)**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        int[] intArray = new int[8];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] =55;
        intArray[5] = 1;
        intArray[6] = -22;

        int newElement = 30;
        intArray[7] = newElement;

        System.out.println(Arrays.toString(intArray));
    }
}
```

**Insert or update an element ar a specific index**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        int[] intArray = new int[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] =55;
        intArray[5] = 1;
        intArray[6] = -22;

        int newElement = 30;
        intArray[1] = newElement;

        System.out.println(Arrays.toString(intArray));
    }
}
```

**Delete an element by setting it to null**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        Integer[] intArray = new Integer[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] =55;
        intArray[5] = 1;
        intArray[6] = -22;

        intArray[1] = null;

        System.out.println(Arrays.toString(intArray));
    }
}
```

**Delete an element by shifting element**

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        Integer[] intArray = new Integer[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] = 55;
        intArray[5] = 1;
        intArray[6] = -22;

        int indexToDelete = 4;

        for (int i = indexToDelete; i < intArray.length -1; i++) {
            intArray[i] = intArray[i + 1];
        }

        intArray[intArray.length - 1] = null;

        System.out.println(Arrays.toString(intArray));

    }
}
```

#### <a name="chapter3part4"></a>Chapter 4 - Part 4: Bubble Sort

In Bubble Sort algorithm

- traverse from left and compare adjacent elements and the higher one is placed at right side
- In this way, the largest element is moved to the rightmost end at first.
- This process is then continued to find the second largest and place it and so on until the data is sorted.

<br>

<div align="center"><img src="img/bubblesort1-w1000-h470.png" width=1000 height=470><br><sub>Bubble Sort Algorithm : Placing the largest element at correct position  - (<a href='https://www.geeksforgeeks.org/bubble-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

<div align="center"><img src="img/bubblesort2-w1000-h470.png" width=1000 height=470><br><sub>Bubble Sort Algorithm : Placing the second largest element at correct position - (<a href='https://www.geeksforgeeks.org/bubble-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

<div align="center"><img src="img/bubblesort3-w1000-h470.png" width=1000 height=470><br><sub>Bubble Sort Algorithm : Placing the remaining elements at their correct positions - (<a href='https://www.geeksforgeeks.org/bubble-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- It is a In-Place algorithm
- O(n^2) - time complexity-quadratic
- it will take 100 steps to sort 10 items, 10000 steps to sort 100 items, 1000000 steps to sort 1000 itens
- Algorithm degrades quickly

```java
public class Main {

    public static void main(String[] args) {

        int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };

        for (int lastUnsortedIndex = intArray.length - 1; lastUnsortedIndex > 0;
                lastUnsortedIndex--) {
            for (int i = 0; i < lastUnsortedIndex; i++) {
                if (intArray[i] > intArray[i + 1]) {
                    swap(intArray, i, i + 1);
                }
            }
        }

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }


    }

    public static void swap(int[] array, int i, int j) {

        if (i == j) {
            return;
        }

        int temp = array[i];
        array[i] = array[j];
        array[j] = temp;

    }
}
```

other solution

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        Integer[] intArray = new Integer[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] = 55;
        intArray[5] = 35;
        intArray[6] = -22;


        for(int j = intArray.length -1; j > 0; j--) {
            for(int i = 0; i < j; i++) {
                if(intArray[i] > intArray[i+1]) {
                    int temp = intArray[i];
                    intArray[i] = intArray[i+1];
                    intArray[i+1] = temp;
                }
            }
        }

        System.out.println(Arrays.toString(intArray));

    }
}
```

If we look at this Bubble Sort, he is a Stable algorithm, because we just make the swap, if ```intArray[i] > intArray[i + 1]```

#### <a name="chapter3part5"></a>Chapter 4 - Part 5: Stable vs Unstable Sort Algorithms

The stability of a sorting algorithm is concerned with how the algorithm treats equal (or repeated) elements. Stable sorting algorithms preserve the relative order of equal elements, while unstable sorting algorithms don’t. In other words, stable sorting maintains the position of two equals elements relative to one another.

<br>

<div align="center"><img src="img/stableunstable-w1380-h390.png" width=1380 height=390><br><sub>Stable and Unstable Sort Algorithms  - (<a href='https://www.baeldung.com/cs/stable-sorting-algorithms'>Work by Baeldung</a>) </sub></div>

<br>

Stable sorting maintains the order of the two equal balls numbered 8, whereas unstable sorting may invert the relative order of the two 8s.

When equal elements are indistinguishable, such as with integers, or more generally, any data where the entire element is the key, stability is not an issue. Stability is also not an issue if all keys are different.

**Where stable sorting algorithms are useful?**

Consider the following dataset of Student Names and their respective class sections.

```
(Dave,A)
(Alice,B)
(Ken,A)
(Eric,B)
(Carol,A)
```

If we sort this data according to name only, then it is highly unlikely that the resulting dataset will be grouped according to sections as well. 

```
(Alice,B)
(Carol,A)
(Dave,A)
(Eric,B)
(Ken,A)
```

So we might have to sort again to obtain the list of students section-wise too. But in doing so, if the sorting algorithm is not stable, we might get a result like this:

```
(Carol,A)
(Dave,A)
(Ken,A)
(Eric,B)
(Alice,B)
```

The dataset is now sorted according to sections, but not according to names. In the name-sorted dataset, the tuple (Alice, B) was before (Eric, B) , but since the sorting algorithm is not stable, the relative order is lost. If on the other hand, we used a stable sorting algorithm, the result would be:

```
(Carol,A)
(Dave,A)
(Ken,A)
(Alice,B)
(Eric,B)
```

**Which sorting algorithms are stable?**

Some Sorting Algorithms are stable by nature, such as Bubble Sort, Insertion Sort, Merge Sort, Count Sort, etc. Comparison-based stable sorts such as Merge Sort and Insertion Sort maintain stability by ensuring that Element A[j]  comes before A[i]  if and only if A[j] < A[i] , here i, j are indices, and i < j . The relative order is preserved if A[i] == A[j]  i.e. A[i]  comes before A[j] 

**Which sorting algorithms are unstable?**

Quick Sort, Heap Sort etc., can be made stable by also taking the position of the elements into consideration. This change may be done in a way that does not compromise a lot on the performance and takes some extra space.

#### <a name="chapter3part6"></a>Chapter 4 - Part 6: Selection Sort

Selection sort is a simple and efficient sorting algorithm that works by repeatedly selecting the smallest (or largest) element from the unsorted portion of the list and moving it to the sorted portion of the list. 

The algorithm repeatedly selects the smallest (or largest) element from the unsorted portion of the list and swaps it with the first element of the unsorted part. This process is repeated for the remaining unsorted portion until the entire list is sorted. 

Lets consider the following array as an example: arr[] = {64, 25, 12, 22, 11}

- For the first position in the sorted array, the whole array is traversed from index 0 to 4 sequentially. The first position where 64 is stored presently, after traversing whole array it is clear that 11 is the lowest value.

- Thus, replace 64 with 11. After one iteration 11, which happens to be the least value in the array, tends to appear in the first position of the sorted list.

<br>

<div align="center"><img src="img/selectionsort1-w1000-h370.png" width=1000 height=370><br><sub>Selection Sort Algorithm | Swapping 1st element with the minimum in array  - (<a href='https://www.geeksforgeeks.org/selection-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- For the second position, where 25 is present, again traverse the rest of the array in a sequential manner.

- After traversing, we found that 12 is the second lowest value in the array and it should appear at the second place in the array, thus swap these values.

<br>

<div align="center"><img src="img/selectionsort2-w1000-h370.png" width=1000 height=370><br><sub>Selection Sort Algorithm | swapping i=1 with the next minimum element  - (<a href='https://www.geeksforgeeks.org/selection-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Now, for third place, where 25 is present again traverse the rest of the array and find the third least value present in the array.

- While traversing, 22 came out to be the third least value and it should appear at the third place in the array, thus swap 22 with element present at third position.

<br>

<div align="center"><img src="img/selectionsort3-w1000-h370.png" width=1000 height=370><br><sub>Selection Sort Algorithm | swapping i=2 with the next minimum element  - (<a href='https://www.geeksforgeeks.org/selection-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Similarly, for fourth position traverse the rest of the array and find the fourth least element in the array

- As 25 is the 4th lowest value hence, it will place at the fourth position.

<br>

<div align="center"><img src="img/selectionsort4-w1000-h370.png" width=1000 height=370><br><sub>Selection Sort Algorithm | swapping i=3 with the next minimum element  - (<a href='https://www.geeksforgeeks.org/selection-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- At last the largest value present in the array automatically get placed at the last position in the array

- The resulted array is the sorted array.

<br>

<div align="center"><img src="img/selectionsort5-w1000-h370.png" width=1000 height=370><br><sub>Selection Sort Algorithm | Required sorted array  - (<a href='https://www.geeksforgeeks.org/selection-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

```java
public class Main {

    public static void main(String[] args) {


        int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };

        for (int lastUnsortedIndex = intArray.length - 1; lastUnsortedIndex > 0;
                lastUnsortedIndex--) {

            int largest = 0;

            for (int i = 1; i <= lastUnsortedIndex; i++) {
                if (intArray[i] > intArray[largest]) {
                    largest = i;
                }
            }

            swap(intArray, largest, lastUnsortedIndex);

        }


        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }


    }

    public static void swap(int[] array, int i, int j) {

        if (i == j) {
            return;
        }

        int temp = array[i];
        array[i] = array[j];
        array[j] = temp;

    }

}
```

Other Solution

```java
public class Solution {
    public static void main(String[] args) throws IOException {
        Integer[] intArray = new Integer[7];

        intArray[0] = 20;
        intArray[1] = 35;
        intArray[2] = -15;
        intArray[3] = 7;
        intArray[4] = 55;
        intArray[5] = 35;
        intArray[6] = -22;


        for(int j = intArray.length -1; j > 0; j--) {
            int largestIndex = 0;
            for(int i = 1; i <= j; i++) {
                if(intArray[largestIndex] < intArray[i]) {
                    largestIndex = i;
                }
            }
            int temp = intArray[j];
            intArray[j] = intArray[largestIndex];
            intArray[largestIndex] = temp;
        }

        System.out.println(Arrays.toString(intArray));

    }
}
```

- It is a In-Place algorithm
- O(n^2) - time complexity-quadratic
- it will take 100 steps to sort 10 items, 10000 steps to sort 100 items, 1000000 steps to sort 1000 itens
- Doesn't require as much swapping as bubble sort
- Unstable algorithm

#### <a name="chapter3part7"></a>Chapter 4 - Part 7: Insertion Sort

Insertion sort is a simple sorting algorithm that works similar to the way you sort playing cards in your hands. 
The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.

To sort an array of size N in ascending order iterate over the array and compare the current element (key) to its predecessor, if the key element is smaller than its predecessor, compare it to the elements before. 
Move the greater elements one position up to make space for the swapped element.

Consider an example: arr[]: {12, 11, 13, 5, 6}

- **First Pass**:
  - Initially, the first two elements of the array are compared in insertion sort.
  - | **12** | **11** | 13 | 5 | 6 |
  - Here, 12 is greater than 11 hence they are not in the ascending order and 12 is not at its correct position. Thus, swap 11 and 12.
  - So, for now 11 is stored in a sorted sub-array.
  - | **11** | **12** | 13 | 5 | 6 |
  
- **Second Pass**:
  -  Now, move to the next two elements and compare them
  - | 11 | **12** | **13** | 5 | 6 |
  - Here, 13 is greater than 12, thus both elements seems to be in ascending order, hence, no swapping will occur. 12 also stored in a sorted sub-array along with 11
  
- **Third Pass**:
  - Now, two elements are present in the sorted sub-array which are 11 and 12
  - Moving forward to the next two elements which are 13 and 5
  - | 11 | 12 | **13** | **5** | 6 |
  - Both 5 and 13 are not present at their correct place so swap them
  - | 11 | 12 | **5** | **13** | 6 |
  - After swapping, elements 12 and 5 are not sorted, thus swap again
  - | 11 | **5** | **12** | 13 | 6 |
  - Here, again 11 and 5 are not sorted, hence swap again
  - | **5** | **11** | 12 | 13 | 6 |
  - Here, 5 is at its correct position
  
- **Fourth Pass**:
  - Now, the elements which are present in the sorted sub-array are 5, 11 and 12
  - Moving to the next two elements 13 and 6
  - | 5 | 11 | 12 | **13** | **6** |
  - Clearly, they are not sorted, thus perform swap between both
  - | 5 | 11 | 12 | **6** | **13** |
  - Now, 6 is smaller than 12, hence, swap again
  - | 5 | 11 | **6** | **12** | 13 |
  - Here, also swapping makes 11 and 6 unsorted hence, swap again
  - | 5 | **6** | **11** | 12 | 13 |
  - Finally, the array is completely sorted.

```java
public class Main {

    public static void main(String[] args) {

        int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };

        for (int firstUnsortedIndex = 1; firstUnsortedIndex < intArray.length;
                firstUnsortedIndex++) {
            int newElement = intArray[firstUnsortedIndex];

            int i;

            for (i = firstUnsortedIndex; i > 0 && intArray[i - 1] > newElement; i--) {
                intArray[i] = intArray[i - 1];
            }

            intArray[i] = newElement;
        }

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }

    }

}
```



- It is a In-Place algorithm
- O(n^2) - time complexity-quadratic
- it will take 100 steps to sort 10 items, 10000 steps to sort 100 items, 1000000 steps to sort 1000 itens
- Stable algorithm

#### <a name="chapter3part8"></a>Chapter 4 - Part 8: Shell Sort

- Variation of Insertion Sort
- Insertion sort chooses which element to insert using a gap of 1
- Shell Sort starts out using a larger gap value
- As the algorithm runs, the gap is reduced
- Goal is to reduce the amount of shifting required

- As the algorithm progresses, the gap is reduced
- The last gap value is always 1
- A gap value of 1 is equivalent to insertion sort
- So, the algorithm does some preliminary work (using gap values greater than 1), and then becomes insertion sort
- By the time we get to insertion sort, the array has been partially sorted, so there's less shifting required

**Knuth Sequence**

| k   | Gap (interval)  | 
| :-- | :--------------:|
| 1   | 1               |
| 2   | 4               |
| 3   | 13              |
| 4   | 40              |
| 5   | 121             |

- Gap is calculated using ((3^k) - 1)/2
- We set k based on the length of the array
- We want the gap to be as close as possible to the length of the array we want to sort, without being greater than the length

**Working of Shell Sort**

- Suppose, we need to sort the following array.

<br>

<div align="center"><img src="img/shellsort1-w1144-h196.png" width=1144 height=196><br><sub>Initial array  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

- We are using the shell's original sequence (N/2, N/4, ...1) as intervals in our algorithm.
  - In the first loop, if the array size is N = 8 then, the elements lying at the interval of N/2 = 4 are compared and swapped if they are not in order.
  - The 0th element is compared with the 4th element.
  - If the 0th element is greater than the 4th one then, the 4th element is first stored in temp variable and the 0th element (ie. greater element) is stored in the 4th position and the element stored in temp is stored in the 0th position.
  
<br>

<div align="center"><img src="img/shellsort2-w1292-h590.png" width=1292 height=590><br><sub>Rearrange the elements at n/2 interval  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

- This process goes on for all the remaining elements.

<br>

<div align="center"><img src="img/shellsort3-w1144-h640.png" width=1144 height=640><br><sub>Rearrange all the elements at n/2 interval  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

- In the second loop, an interval of N/4 = 8/4 = 2 is taken and again the elements lying at these intervals are sorted.


<br>

<div align="center"><img src="img/shellsort4-w1144-h344.png" width=1144 height=344><br><sub>Rearrange the elements at n/4 interval  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

- You might get confused at this point.

<br>

<div align="center"><img src="img/shellsort5-w1144-h344.png" width=1144 height=344><br><sub>All the elements in the array lying at the current interval are compared.  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

- The elements at 4th and 2nd position are compared. The elements at 2nd and 0th position are also compared. All the elements in the array lying at the current interval are compared.

- The same process goes on for remaining elements

<br>

<div align="center"><img src="img/shellsort6-w1144-h788.png" width=1144 height=788><br><sub>Rearrange all the elements at n/4 interval  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

- Finally, when the interval is N/8 = 8/8 =1 then the array elements lying at the interval of 1 are sorted. The array is now completely sorted.

<br>

<div align="center"><img src="img/shellsort7-w1144-h1380.png" width=1144 height=1380><br><sub>Rearrange the elements at n/8 interval  - (<a href='https://www.programiz.com/dsa/shell-sort'>Work by Programiz</a>) </sub></div>

<br>

```java
public class Main {

    public static void main(String[] args) {

	    int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };

        for (int gap = intArray.length / 2; gap > 0; gap /= 2) {


            for (int i = gap; i < intArray.length; i++) {
                int newElement = intArray[i];

                int j = i;

                while (j >= gap && intArray[j - gap] > newElement) {
                    intArray[j] = intArray[j - gap];
                    j -= gap;
                }

                intArray[j] = newElement;


            }

        }

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }
    }

}
```

- In-Place algorithm
- Dificult to nail down the time complexity because it will depend on the gap. Worst case: O(n^2), but it can perform much better than that
- Doesn't require as much shifting as insertion sort, so it usuaaly performs better
- Unstable algorithm

#### <a name="chapter3part9"></a>Chapter 4 - Part 9: Recursion

**Factorial Algorithm**

- If num is equal to 0, the factorial is 1. Stop. We have the result.
Otherwise...

- set multiplier to 1
- set factorial to 1
- while multiplier is not equal to num, do steps 5 and 6
- multiply factorial by multiplier and assign the result to factorial
- add 1 to multiplier
- Step. The result is factorial


```java
public class Main {

    public static void main(String[] args) {

        System.out.println(iterativeFactorial(3));
        System.out.println(recursiveFactorial(3));
    }

    // 1! = 1 * 0! = 1
    // 2! = 2 * 1 = 2 * 1!
    // 3! = 3 * 2 * 1 = 3 * 2!
    // 4! = 4 * 3 * 2 * 1 = 4 * 3!

    // n! = n *(n - 1)!








    public static int recursiveFactorial(int num) {

        if (num == 0) {
            return 1;
        }

        return num * recursiveFactorial(num - 1);

    }

    public static int iterativeFactorial(int num) {

        if (num == 0) {
            return 1;
        }

        int factorial = 1;
        for (int i = 1; i <= num; i++) {
            factorial *= i;
        }

        return factorial;

    }
}
```

#### <a name="chapter3part10"></a>Chapter 4 - Part 10: Merge Sort

- Divide and conquer algorithm
- Recursive algorithm
- Two phases: Splitting and Merging
- Splitting phase leads to faster sorting during the Merging phase
- Splitting is logical. We don't create new arrays.

**Splitting Phase**

- Start with unsorted array.
- Divide the array into two arrays, which are unsorted. The first array is the left array, and the second array is the right array.
- Split the left and right arrays into two arrays each
- Keep splitting until all the arrays have only one element each - the arrays are sorted

**Merging Phase**

- Merge every left/right pair of sibling arrays into a sorted array
- After the first merge, we'll have a bunch of 2-element sorted arrays
- Then merge those sorted arrays (left/right siblings) to end up with a bunch of 4-element sorted arrays
- Repeat until you have a single sorted array
- Not in-place. Uses temporary arrays.

**Merging process**

- We merge sibling left and right arrays
- We create a temporary array large enough to hold all the elements in the arrays we're merging
- We set i to the first index of the left array, and j to the first index of the right array
- We compare left[i] to right[j]. If left is smaller, we copy it to the temp array and increment i by 1. If right is smaller, we copy it to the temp array and increment j by 1.
- We repeat this process until all elements in the two arrays have been processed
- At this point, the temporary array contains the merged values in sorted order
- We then copy this temporary array back to the original input array, at the correct positions
- If the left array is at positions x to y, and the right array is at positions y + 1 to z, then after the copy, positions x to z will be sorted in the original array


<br>

<div align="center"><img src="img/mergesort1-w1001-h471.png" width=1001 height=471><br><sub>Merge Sort: Divide the array into two halves - (<a href='https://www.geeksforgeeks.org/merge-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

<div align="center"><img src="img/mergesort2-w1001-h471.png" width=1001 height=471><br><sub>Merge Sort: Divide the subarrays into two halves (unit length subarrays here) - (<a href='https://www.geeksforgeeks.org/merge-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

<div align="center"><img src="img/mergesort3-w1001-h471.png" width=1001 height=471><br><sub>Merge Sort: Merge the unit length subarrys into sorted subarrays - (<a href='https://www.geeksforgeeks.org/merge-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

<div align="center"><img src="img/mergesort4-w1001-h471.png" width=1001 height=471><br><sub>Merge Sort: Merge the sorted subarrys to get the sorted array - (<a href='https://www.geeksforgeeks.org/merge-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>


```java
public class Main {

    public static void main(String[] args) {
        int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };

        mergeSort(intArray, 0, intArray.length);

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }
    }

    // { 20, 35, -15, 7, 55, 1, -22 }
    public static void mergeSort(int[] input, int start, int end) {

        if (end - start < 2) {
            return;
        }

        int mid = (start + end) / 2;
        mergeSort(input, start, mid);
        mergeSort(input, mid, end);
        merge(input, start, mid, end);
    }

    // { 20, 35, -15, 7, 55, 1, -22 }
    public static void merge(int[] input, int start, int mid, int end) {

        if (input[mid - 1] <= input[mid]) {
            return;
        }

        int i = start;
        int j = mid;
        int tempIndex = 0;

        int[] temp = new int[end - start];
        while (i < mid && j < end) {
            temp[tempIndex++] = input[i] <= input[j] ? input[i++] : input[j++];
        }

        System.arraycopy(input, i, input, start + tempIndex, mid - i);
        System.arraycopy(temp, 0, input, start, tempIndex);


    }

}
```

- Not an in-place algorithm 

- O(nlog.n) - base 2.We're repeatedly dividing the array in half during the splitting phase

- Stable algorithm
  

#### <a name="chapter3part11"></a>Chapter 4 - Part 11: Quick Sort

- Divide and conquer algorithm
- Recursive algorithm
- Uses a pivot element to partition the array into two parts
- Elements < pivot to its left, elements > pivot to its right
- Pivot will then be in its correct sorted position

- Process is now repeated fot the left array and right array
- Eventually, every element has been the pivot, so every element will be in its correct sorted position
- As with merge sort, we'll end up partitioning the array into a series of 1-element arrays
- Does this in-place(unlike merge sort)

- Compare 10 with the pivot and as it is less than pivot arrange it accrodingly.

<br>

<div align="center"><img src="img/quicksort1-w1000-h370.png" width=1000 height=370><br><sub>Partition in QuickSort: Compare pivot with 10 - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Compare 80 with the pivot. It is greater than pivot.

<br>

<div align="center"><img src="img/quicksort2-w1000-h370.png" width=1000 height=370><br><sub>Partition in QuickSort: Compare pivot with 80 - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Compare 30 with pivot. It is less than pivot so arrange it accordingly.

<br>

<div align="center"><img src="img/quicksort3-w1000-h370.png" width=1000 height=370><br><sub>Partition in QuickSort: Compare pivot with 30 - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Compare 90 with the pivot. It is greater than the pivot.

<br>

<div align="center"><img src="img/quicksort4-w1000-h370.png" width=1000 height=370><br><sub>Partition in QuickSort: Compare pivot with 90 - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Arrange the pivot in its correct position.

<br>

<div align="center"><img src="img/quicksort5-w1000-h370.png" width=1000 height=370><br><sub>Partition in QuickSort: Place pivot in its correct position - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

**Illustration of Quicksort:**

As the partition process is done recursively, it keeps on putting the pivot in its actual position in the sorted array. Repeatedly putting pivots in their actual position makes the array sorted.

Follow the below images to understand how the recursive implementation of the partition algorithm helps to sort the array.

- Initial partition on the main array:

<br>

<div align="center"><img src="img/quicksort6-w1000-h370.png" width=1000 height=370><br><sub>Quicksort: Performing the partition - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Partitioning of the subarrays:

<br>

<div align="center"><img src="img/quicksort7-w1000-h370.png" width=1000 height=370><br><sub>Quicksort: Performing the partition - (<a href='https://www.geeksforgeeks.org/quick-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>


```java
public class Main {

    public static void main(String[] args) {
        int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };

        quickSort(intArray, 0, intArray.length);

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }
    }

    public static void quickSort(int[] input, int start, int end) {
        if (end - start < 2) {
            return;
        }

        int pivotIndex = partition(input, start, end);
        quickSort(input, start, pivotIndex);
        for (int i = 0; i < input.length; i++) {
            System.out.println(input[i]);
        }
        quickSort(input, pivotIndex + 1, end);
    }

    public static int partition(int[] input, int start, int end) {
        // This is using the first element as the pivot
        int pivot = input[start];
        int i = start;
        int j = end;

        while (i < j) {

            // NOTE: empty loop body
            while (i < j && input[--j] >= pivot);
            if (i < j) {
                input[i] = input[j];
            }

            // NOTE: empty loop body
            while (i < j && input[++i] <= pivot);
            if (i < j) {
                input[j] = input[i];
            }

        }

        input[j] = pivot;
        return j;

    }
}
```

- In-place algorithm 

- O(nlog.n) - base 2.We're repeatedly partioning the array into two halves

- Unstable algorithm

#### <a name="chapter3part12"></a>Chapter 4 - Part 12: Counting Sort

- Makes assumptions about the data
- Doesn't use comparisons
- Counts the number of occurences of each value
- Only works with non-negative discrete values (can't work with floats, strings)
- Values must be within a specific range

- Find out the maximum element from the given array.

<br>

<div align="center"><img src="img/countingsort1-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Initialize a countArray[] of length max+1 with all elements as 0. This array will be used for storing the occurrences of the elements of the input array

<br>

<div align="center"><img src="img/countingsort2-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- In the countArray[], store the count of each unique element of the input array at their respective indices.
- For Example: The count of element 2 in the input array is 2. So, store 2 at index 2 in the countArray[]. Similarly, the count of element 5 in the input array is 1, hence store 1 at index 5 in the countArray[].

<br>

<div align="center"><img src="img/countingsort3-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Store the cumulative sum or prefix sum of the elements of the countArray[] by doing countArray[i] = countArray[i – 1] + countArray[i]. 
This will help in placing the elements of the input array at the correct index in the output array.

<br>

<div align="center"><img src="img/countingsort4-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Iterate from end of the input array and because traversing input array from end preserves the order of equal elements, which eventually makes this sorting algorithm stable.
- Update outputArray[ countArray[ inputArray[i] ] – 1] = inputArray[i].
- Also, update countArray[ inputArray[i] ] = countArray[ inputArray[i] ]– -.

<br>

<div align="center"><img src="img/countingsort5-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- For i = 6,
- Update outputArray[ countArray[ inputArray[6] ] – 1] = inputArray[6]
- Also, update countArray[ inputArray[6] ] = countArray[ inputArray[6] ]- –

<br>

<div align="center"><img src="img/countingsort6-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- For i = 5,
- Update outputArray[ countArray[ inputArray[5] ] – 1] = inputArray[5]
- Also, update countArray[ inputArray[5] ] = countArray[ inputArray[5] ]- –

<br>

<div align="center"><img src="img/countingsort7-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- For i = 4,
- Update outputArray[ countArray[ inputArray[4] ] – 1] = inputArray[4]
- Also, update countArray[ inputArray[4] ] = countArray[ inputArray[4] ]- –

<br>

<div align="center"><img src="img/countingsort8-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>


- For i = 3,
- Update outputArray[ countArray[ inputArray[3] ] – 1] = inputArray[3]
- Also, update countArray[ inputArray[3] ] = countArray[ inputArray[3] ]- –

<br>

<div align="center"><img src="img/countingsort9-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- For i = 2,
- Update outputArray[ countArray[ inputArray[2] ] – 1] = inputArray[2]
- Also, update countArray[ inputArray[2] ] = countArray[ inputArray[2] ]- –

<br>

<div align="center"><img src="img/countingsort10-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- For i = 1,
- Update outputArray[ countArray[ inputArray[1] ] – 1] = inputArray[1]
- Also, update countArray[ inputArray[1] ] = countArray[ inputArray[1] ]- –

<br>

<div align="center"><img src="img/countingsort11-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

-  For i = 0,
- Update outputArray[ countArray[ inputArray[0] ] – 1] = inputArray[0]
- Also, update countArray[ inputArray[0] ] = countArray[ inputArray[0] ]- –

<br>

<div align="center"><img src="img/countingsort12-w1000-h498.png" width=1000 height=498><br><sub> - (<a href='https://www.geeksforgeeks.org/counting-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>


```java
public class Main {

    public static void main(String[] args) {
        int[] intArray = { 2, 5, 9, 8, 2, 8, 7, 10, 4, 3 };

        countingSort(intArray, 1, 10);

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }
    }

    public static void countingSort(int[] input, int min, int max) {

        int[] countArray = new int[(max - min) + 1];

        for (int i = 0; i < input.length; i++) {
            countArray[input[i] - min]++;
        }

        int j = 0;
        for (int i = min; i <= max; i++) {
            while (countArray[i - min] > 0) {
                input[j++] = i;
                countArray[i - min]--;
            }
        }

    }
}
```

- Not an in-place algorithm
- O(n) - can achieve this because we're making assumptions about the data we're sorting
- If we want the sort to be stable, we have to do some extra steps


#### <a name="chapter3part13"></a>Chapter 4 - Part 13: Radix Sort

- Makes assumptions about the data
- Data must have same radix and width
- Because of this, data must be integers or strings
- Sort based on each individual digit or letter position
- Start at the rightmost position
- Must use a stable sort algorithm at each stage

<br>

<div align="center"><img src="img/radixsort1-w1000-h400.png" width=1000 height=400><br><sub>How does Radix Sort Algorithm work | Step 1 - (<a href='https://www.geeksforgeeks.org/radix-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Find the largest element in the array, which is 802. It has three digits, so we will iterate three times, once for each significant place.

- Sort the elements based on the unit place digits (X=0). We use a stable sorting technique, such as counting sort, to sort the digits at each significant place.

- Sorting based on the unit place:
  - Perform counting sort on the array based on the unit place digits.
  - The sorted array based on the unit place is [170, 90, 802, 2, 24, 45, 75, 66].
  
<br>

<div align="center"><img src="img/radixsort2-w1000-h400.png" width=1000 height=400><br><sub>How does Radix Sort Algorithm work | Step 2 - (<a href='https://www.geeksforgeeks.org/radix-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Sort the elements based on the tens place digits.
- Sorting based on the tens place:
  - Perform counting sort on the array based on the tens place digits.
  - The sorted array based on the tens place is [802, 2, 24, 45, 66, 170, 75, 90].
  
<br>

<div align="center"><img src="img/radixsort3-w1000-h400.png" width=1000 height=400><br><sub>How does Radix Sort Algorithm work | Step 3 - (<a href='https://www.geeksforgeeks.org/radix-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- Sort the elements based on the hundreds place digits.
- Sorting based on the hundreds place:
  - Perform counting sort on the array based on the hundreds place digits.
  - The sorted array based on the hundreds place is [2, 24, 45, 66, 75, 90, 170, 802].
  
<br>

<div align="center"><img src="img/radixsort4-w1000-h400.png" width=1000 height=400><br><sub>How does Radix Sort Algorithm work | Step 4 - (<a href='https://www.geeksforgeeks.org/radix-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

- The array is now sorted in ascending order.
- The final sorted array using radix sort is [2, 24, 45, 66, 75, 90, 170, 802].

<br>

<div align="center"><img src="img/radixsort5-w1000-h400.png" width=1000 height=400><br><sub>How does Radix Sort Algorithm work | Step 5 - (<a href='https://www.geeksforgeeks.org/radix-sort/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

```java
public class Main {

    public static void main(String[] args) {

        int[] radixArray = { 4725, 4586, 1330, 8792, 1594, 5729 };

        radixSort(radixArray, 10, 4);

        for (int i = 0; i < radixArray.length; i++) {
            System.out.println(radixArray[i]);
        }
    }

    public static void radixSort(int[] input, int radix, int width) {
        for (int i = 0; i < width; i++) {
            radixSingleSort(input, i, radix);
        }
    }

    public static void radixSingleSort(int[] input, int position, int radix) {

        int numItems = input.length;
        int[] countArray = new int[radix];

        for (int value: input) {
            countArray[getDigit(position, value, radix)]++;
        }
        // Adjust the count array
        for (int j = 1; j < radix; j++) {
            countArray[j] += countArray[j - 1];
        }

        int[] temp = new int[numItems];
        for (int tempIndex = numItems - 1; tempIndex >= 0; tempIndex--) {
            temp[--countArray[getDigit(position, input[tempIndex], radix)]] =
                    input[tempIndex];
        }

        for (int tempIndex = 0; tempIndex < numItems; tempIndex++) {
            input[tempIndex] = temp[tempIndex];
        }

    }


    public static int getDigit(int position, int value, int radix) {
        return value / (int) Math.pow(radix, position) % radix;
    }

}
```

- Counting sort is often used as the sort algorithm ofr radix sort - must be stable counting sort
- O(n) - can achieve this because we're making assumptions about the data we're sorting
- Even so, it often runs slower than O(n.log.n) algorithms because of the overhead involved 
- In-place depends on which sort algorithm you use
- Stable algorithm

#### <a name="chapter3part14"></a>Chapter 4 - Part 14: Sorting Arrays using JDK

A useful class to use to make operations in Arrays in Java is the Arrays.class

We can see the operations in the [Java Arrays Doc](https://docs.oracle.com/javase/8/docs/api/java/util/Arrays.html)

```java
public class Main {

    public static void main(String[] args) {
        int[] intArray = { 20, 35, -15, 7, 55, 1, -22 };
		
		
        Arrays.parallelSort(intArray);

        for (int i = 0; i < intArray.length; i++) {
            System.out.println(intArray[i]);
        }
    }
}
```

## <a name="chapter4"></a>Chapter 4: Lists in Java
  
#### <a name="chapter4part1"></a>Chapter 4 - Part 1: Introduction to Lists

The List interface is found in ```java.util``` package and inherits the ```Collection interface```. It is a factory of the ListIterator interface. Through the ListIterator, we can iterate the list in forward and backward directions. The implementation classes of the List interface are ```ArrayList```, ```LinkedList```, ```Stack```, and ```Vector```. ```ArrayList``` and ```LinkedList``` are widely used in Java programming. The Vector class is deprecated since Java 5.

[Java List Doc](https://docs.oracle.com/javase/8/docs/api/java/util/List.html)

<br>

<div align="center"><img src="img/listcollection-w768-h384.png" width=768 height=384><br><sub>List and ArrayList in Java Collection Framework - (<a href='https://www.geeksforgeeks.org/list-interface-java-examples/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

<div align="center"><img src="img/listimplementation-w768-h384.png" width=768 height=384><br><sub> - (<a href='https://www.geeksforgeeks.org/list-interface-java-examples/'>Work by Geeks for Geeks</a>) </sub></div>

<br>

The list is an abstract data type. A list isn't a concrete data structure, it's an abstract data type nnd when it comes to abstract data types, normally there's an interface involved and list is no exception.
Some the lists that we're gonna look all implement the ```java.util.list interface```. Classes that implement the list interface represent an ordered collection also known as a sequence. Some of them is Array List, Linked List, Vector.

**Abstract Data Type**

- Doesn´t dictate how the data is organized
- Dictates the operations you can perform
- Concrete data structure is usually a concrete class
- Abstract data type is usually an interface

If you want to implement the list interface, you want to create a custom implementation rather than starting with list itself and implementing that, it's a good idea to instead extend abstract list and abstract sequential list because there are scoledo implementations of the list interface and so they kind of give you a head start and all you have to do is override the methods that you specifically want to implement if you want custom behaviour. So if you are going to implement a custom list, its a good idea to extend one of these two classes.

**Declaration of Java List Interface**

```java
public interface List<E> extends Collection<E> ; 
```

Since List is an interface, objects cannot be created of the type list. We always need a class that implements this List in order to create an object. And also, after the introduction of Generics in Java 1.5, it is possible to restrict the type of object that can be stored in the List. Just like several other user-defined ‘interfaces’ implemented by user-defined ‘classes’, List is an ‘interface’, implemented by the ArrayList class, pre-defined in java.util package.

**Syntax of Java List**

This type of safelist can be defined as:

```java
List<Obj> list = new ArrayList<Obj> (); 
```

Obj is the type of the object to be stored in List

**Example of Java List**

```java
// Java program to Demonstrate List Interface
 
// Importing all utility classes
import java.util.*;
 
// Main class
// ListDemo class
class GFG {
 
    // Main driver method
    public static void main(String[] args)
    {
 
        // Creating an object of List interface
        // implemented by the ArrayList class
        List<Integer> l1 = new ArrayList<Integer>();
 
        // Adding elements to object of List interface
        // Custom inputs
 
        l1.add(0, 1);
        l1.add(1, 2);
 
        // Print the elements inside the object
        System.out.println(l1);
 
        // Now creating another object of the List
        // interface implemented ArrayList class
        // Declaring object of integer type
        List<Integer> l2 = new ArrayList<Integer>();
 
        // Again adding elements to object of List interface
        // Custom inputs
        l2.add(1);
        l2.add(2);
        l2.add(3);
 
        // Will add list l2 from 1 index
        l1.addAll(1, l2);
 
        System.out.println(l1);
 
        // Removes element from index 1
        l1.remove(1);
 
        // Printing the updated List 1
        System.out.println(l1);
 
        // Prints element at index 3 in list 1
        // using get() method
        System.out.println(l1.get(3));
 
        // Replace 0th element with 5
        // in List 1
        l1.set(0, 5);
 
        // Again printing the updated List 1
        System.out.println(l1);
    }
} 
```

**Operations in a Java List Interface**

- Adding elements to List class using add() method
- In order to add an element to the list, we can use the add() method. This method is overloaded to perform multiple operations based on different parameters.
  - **add(Object)**: This method is used to add an element at the end of the List.
  - **add(int index, Object)**: This method is used to add an element at a specific index in the List

```java
// Java Program to Add Elements to a List
 
// Importing all utility classes
import java.util.*;
 
// Main class
class GFG {
 
    // Main driver method
    public static void main(String args[])
    {
        // Creating an object of List interface,
        // implemented by ArrayList class
        List<String> al = new ArrayList<>();
 
        // Adding elements to object of List interface
        // Custom elements
        al.add("Geeks");
        al.add("Geeks");
        al.add(1, "For");
 
        // Print all the elements inside the
        // List interface object
        System.out.println(al);
    }
}
```

- Updating elements in List class using set() method
- After adding the elements, if we wish to change the element, it can be done using the set() method. Since List is indexed, the element which we wish to change is referenced by the index of the element. Therefore, this method takes an index and the updated element which needs to be inserted at that index. 

```java
// Java Program to Update Elements in a List
 
// Importing utility classes
import java.util.*;
 
// Main class
class GFG {
 
    // Main driver method
    public static void main(String args[])
    {
        // Creating an object of List interface
        List<String> al = new ArrayList<>();
 
        // Adding elements to object of List class
        al.add("Geeks");
        al.add("Geeks");
        al.add(1, "Geeks");
 
        // Display theinitial elements in List
        System.out.println("Initial ArrayList " + al);
 
        // Setting (updating) element at 1st index
        // using set() method
        al.set(1, "For");
 
        // Print and display the updated List
        System.out.println("Updated ArrayList " + al);
    }
}
```

- Searching for elements using indexOf(), lastIndexOf methods
- Searching for elements in the List interface is a common operation in Java programming. The List interface provides several methods to search for elements, such as the indexOf(), lastIndexOf() methods.
- The indexOf() method returns the index of the first occurrence of a specified element in the list, while the lastIndexOf() method returns the index of the last occurrence of a specified element.
  - **indexOf(element)**: Returns the index of the first occurrence of the specified element in the list, or -1 if the element is not found
  - **lastIndexOf(element)**: Returns the index of the last occurrence of the specified element in the list, or -1 if the element is not found

```java
import java.util.ArrayList;
import java.util.List;
 
public class ListExample {
    public static void main(String[] args)
    {
        // create a list of integers
        List<Integer> numbers = new ArrayList<>();
 
        // add some integers to the list
        numbers.add(1);
        numbers.add(2);
        numbers.add(3);
        numbers.add(2);
 
        // use indexOf() to find the first occurrence of an
        // element in the list
        int index = numbers.indexOf(2);
        System.out.println(
            "The first occurrence of 2 is at index "
            + index);
 
        // use lastIndexOf() to find the last occurrence of
        // an element in the list
        int lastIndex = numbers.lastIndexOf(2);
        System.out.println(
            "The last occurrence of 2 is at index "
            + lastIndex);
    }
}
```

- Removing elements using remove() method
- In order to remove an element from a list, we can use the remove() method. This method is overloaded to perform multiple operations based on different parameters. They are:
  - **remove(Object)**: This method is used to simply remove an object from the List. If there are multiple such objects, then the first occurrence of the object is removed.
  - **remove(int index)**: Since a List is indexed, this method takes an integer value which simply removes the element present at that specific index in the List. After removing the element, all the elements are moved to the left to fill the space and the indices of the objects are updated.

```java
   
// Java Program to Remove Elements from a List
 
// Importing List and ArrayList classes
// from java.util package
import java.util.ArrayList;
import java.util.List;
 
// Main class
class GFG {
 
    // Main driver method
    public static void main(String args[])
    {
 
        // Creating List class object
        List<String> al = new ArrayList<>();
 
        // Adding elements to the object
        // Custom inputs
        al.add("Geeks");
        al.add("Geeks");
 
        // Adding For at 1st indexes
        al.add(1, "For");
 
        // Print the initialArrayList
        System.out.println("Initial ArrayList " + al);
 
        // Now remove element from the above list
        // present at 1st index
        al.remove(1);
 
        // Print the List after removal of element
        System.out.println("After the Index Removal " + al);
 
        // Now remove the current object from the updated
        // List
        al.remove("Geeks");
 
        // Finally print the updated List now
        System.out.println("After the Object Removal "
                           + al);
    }
}
```

- Accessing Elements in List class using get() method
- In order to access an element in the list, we can use the get() method, which returns the element at the specified index
  - **get(int index)**: This method returns the element at the specified index in the list.

```java
// Java Program to Access Elements of a List
 
// Importing all utility classes
import java.util.*;
 
// Main class
class GFG {
    // Main driver method
    public static void main(String args[])
    {
        // Creating an object of List interface,
        // implemented by ArrayList class
        List<String> al = new ArrayList<>();
 
        // Adding elements to object of List interface
        al.add("Geeks");
        al.add("For");
        al.add("Geeks");
 
        // Accessing elements using get() method
        String first = al.get(0);
        String second = al.get(1);
        String third = al.get(2);
 
        // Printing all the elements inside the
        // List interface object
        System.out.println(first);
        System.out.println(second);
        System.out.println(third);
        System.out.println(al);
    }
}
```

- Checking if an element is present in the List class using contains() method
- In order to check if an element is present in the list, we can use the contains() method. This method returns true if the specified element is present in the list, otherwise, it returns false.
  - **contains(Object)**: This method takes a single parameter, the object to be checked if it is present in the list.

```java
// Java Program to Check if an Element is Present in a List
 
// Importing all utility classes
import java.util.*;
 
// Main class
class GFG {
    // Main driver method
    public static void main(String args[])
    {
        // Creating an object of List interface,
        // implemented by ArrayList class
        List<String> al = new ArrayList<>();
 
        // Adding elements to object of List interface
        al.add("Geeks");
        al.add("For");
        al.add("Geeks");
 
        // Checking if element is present using contains()
        // method
        boolean isPresent = al.contains("Geeks");
 
        // Printing the result
        System.out.println("Is Geeks present in the list? "
                           + isPresent);
    }
}
```

Now, let's see some operations in List and the time complexity

| Operation                                        | Time Complexity        | 
| :----------------------------------------------- | :---------------------:|
| Adding Element in List Interface                 | O(1) - Constant time   |
| Remove Element from List Interface               | O(n) - Linear Time     |
| Replace Element in List Interface                | O(n)                   |
| Traversing List Interface                        | O(n)                   |   

#### <a name="chapter4part2"></a>Chapter 4 - Part 2: Array Lists

Java ArrayList is a part of the Java collection framework and it is a class of java.util package. It provides us with dynamic arrays in Java. Though, it may be slower than standard arrays but can be helpful in programs where lots of manipulation in the array is needed. This class is found in java.util package. The main advantage of Java ArrayList is, if we declare an array then we need to mention the size, but in ArrayList, it is not needed to mention the size of ArrayList. If you want to mention the size then you can do it.

[Java ArrayList Doc](https://docs.oracle.com/javase/8/docs/api/java/util/ArrayList.html)

ArrayList is a Java class implemented using the List interface. Java ArrayList, as the name suggests, provides the functionality of a dynamic array where the size is not fixed as an array. Also, as a part of the Collection framework, it has many features not available with arrays.

**Java ArrayList Example**

```java

```

**Important Features of ArrayList in Java**

- ArrayList inherits AbstractList class and implements the List interface.
- ArrayList is initialized by size. However, the size is increased automatically if the collection grows or shrinks if the objects are removed from the collection.
- Java ArrayList allows us to randomly access the list.
- ArrayList can not be used for primitive types, like int, char, etc. We need a wrapper class for such cases.
- ArrayList in Java can be seen as a vector in C++.
- ArrayList is not Synchronized. Its equivalent synchronized class in Java is Vector.

**Some Key Points of ArrayList**

- ArrayList is Underlined data Structure Resizable Array or Growable Array.
- ArrayList Duplicates Are Allowed.
- Insertion Order is Preserved.
- Heterogeneous objects are allowed.
- Null insertion is possible.

Now, let's see some operations in ArrayList and the time complexity

| Operation                                        | Time Complexity        | 
| :----------------------------------------------- | :---------------------:|
| Inserting Element in ArrayList                   | O(1) - Constant time   |
| Removing Element from ArrayList                  | O(n) - Linear Time     |
| Replacing Elements in ArrayList                  | O(1)                   |
| Traversing Elements in ArrayList                 | O(n)                   |

**Advantages of Java ArrayList**
- Dynamic size: ArrayList can dynamically grow and shrink in size, making it easy to add or remove elements as needed.
- Easy to use: ArrayList is simple to use, making it a popular choice for many Java developers.
- Fast access: ArrayList provides fast access to elements, as it is implemented as an array under the hood.
- Ordered collection: ArrayList preserves the order of elements, allowing you to access elements in the order they were added.
- Supports null values: ArrayList can store null values, making it useful in cases where the absence of a value needs to be represented.

**Disadvantages of Java ArrayList**
- Slower than arrays: ArrayList is slower than arrays for certain operations, such as inserting elements in the middle of the list.
- Increased memory usage: ArrayList requires more memory than arrays, as it needs to maintain its dynamic size and handle resizing.
- Not thread-safe: ArrayList is not thread-safe, meaning that multiple threads may access and modify the list concurrently, leading to potential race conditions and data corruption.
- Performance degradation: ArrayList’s performance may degrade as the number of elements in the list increases, especially for operations such as searching for elements or inserting elements in the middle of the list.

#### <a name="chapter4part3"></a>Chapter 4 - Part 3: Vectors

#### <a name="chapter4part4"></a>Chapter 4 - Part 4: Singly Linked Lists

#### <a name="chapter4part5"></a>Chapter 4 - Part 5: Doubly Linked Lists

#### <a name="chapter4part6"></a>Chapter 4 - Part 6: JDK LinkedList Class

## <a name="chapter5"></a>Chapter 5: Stacks in Java
  
#### <a name="chapter5part1"></a>Chapter 5 - Part 1: Introduction to Stacks

## <a name="chapter6"></a>Chapter 6: Queues in Java
  
#### <a name="chapter6part1"></a>Chapter 6 - Part 1: Introduction to Queues

## <a name="chapter7"></a>Chapter 7: Hashtables in Java
  
#### <a name="chapter7part1"></a>Chapter 7 - Part 1: Introduction to Hashtables

## <a name="chapter8"></a>Chapter 8: Search Algorithms
  
#### <a name="chapter8part1"></a>Chapter 8 - Part 1: Introduction to Search Algorithms
	
## <a name="chapter9"></a>Chapter 9: Trees in Java
  
#### <a name="chapter9part1"></a>Chapter 9 - Part 1: Introduction to Trees

## <a name="chapter10"></a>Chapter 10: Heaps in Java
  
#### <a name="chapter10part1"></a>Chapter 10 - Part 1: Introduction to Heaps

## <a name="chapter11"></a>Chapter 11: Sets in Java
  
#### <a name="chapter11part1"></a>Chapter 11 - Part 1: Introduction to Sets
