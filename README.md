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

Some Sorting Algorithms are stable by nature, such as Bubble Sort, Insertion Sort, Merge Sort, Count Sort, etc. Comparison-based stable sorts such as Merge Sort and Insertion Sort maintain stability by ensuring that Element A[j]  comes before A[i]  if and only if A[j] < A[i] , here i, j are indices, and i < j . The relative order is preserved if A[i] \equiv A[j]  i.e. A[i]  comes before A[j] 

**Which sorting algorithms are unstable?**

Quick Sort, Heap Sort etc., can be made stable by also taking the position of the elements into consideration. This change may be done in a way that does not compromise a lot on the performance and takes some extra space, possibly \theta(n).

#### <a name="chapter3part6"></a>Chapter 4 - Part 6: Selection Sort

#### <a name="chapter3part7"></a>Chapter 4 - Part 7: Insertion Sort

#### <a name="chapter3part8"></a>Chapter 4 - Part 8: Shell Sort

#### <a name="chapter3part9"></a>Chapter 4 - Part 9: Recursion

#### <a name="chapter3part10"></a>Chapter 4 - Part 10: Merge Sort

#### <a name="chapter3part11"></a>Chapter 4 - Part 11: Quick Sort

#### <a name="chapter3part12"></a>Chapter 4 - Part 12: Counting Sort

#### <a name="chapter3part13"></a>Chapter 4 - Part 13: Radix Sort
