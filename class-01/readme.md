# Class- 01
## 17/7/2021
## What is an Algorithm?
An algorithm is a set of instructions for solving a problem or accomplishing a task.

## What is Data Structure?
Data Structure is a way of collecting and organising data in such a way that we can perform operations on these data in an effective way.

Basic Data Structure Discussion 1. Array 2. List in Python


## Difference between List and Array in Python

- List:A list in Python is a collection of items which can contain elements of multiple data types, which may be either numeric, character logical values, etc. It is an ordered collection supporting negative indexing. A list can be created using [] containing data values.
    Example:-

Question | Output
------------ | -------------
sample_list = [1,"Yash",['a','e']]|
print(sample_list)                | [1, 'Yash', ['a', 'e']]

The first element is an integer, the second a string and the third is an list of characters.

- Array:An array is a vector containing homogeneous elements i.e. belonging to the same data type. Elements are allocated with contiguous memory locations allowing easy modification, that is, addition, deletion, accessing of elements. In Python, we have to use the array module to declare arrays. If the elements of an array belong to different data types, an exception “Incompatible data types” is thrown.
Example:

Question | Output
------------ | -------------
import array |  
sample_array = array.array('i', [1, 2, 3])  |1               
for i in sample_array:                      |2
print(i)                                    |3

## Data Struectur Asymptotic Notation:

Asymptotic Notations are the expressions that are used to represent the complexity of an algorithm.
There are three types of analysis that we perform on a particular algorithm.
- Best Case: In which we analyse the performance of an algorithm for the input, for which the algorithm takes less time or space.
- Worst Case: In which we analyse the performance of an algorithm for the input, for which the algorithm takes long time or space.
- Average Case: In which we analyse the performance of an algorithm for the input, for which the algorithm takes time or space that lies between best and worst case.

##  Types of Data Structure Asymptotic Notation
### 1. Big-O Notation (Ο) – 
      Big O notation specifically describes worst case scenario.
      (i) O(1):Big O notation O(1) represents the complexity of an algorithm that always execute in same time or space regardless of the input data.
      Exapmle :- Accessing array index(int num = arr[5])

      (ii)O(n):Big O notation O(N) represents the complexity of an algorithm, whose performance will grow linearly (in direct proportion) to the size of the input data. 
      Example:- The execution time will depend on the size of array. When the size of the array increases, the execution time will also increase in the same proportion (linearly)
       Traversing an array 
      (iii)O(n^2):Big O notation O(n^2) represents the complexity of an algorithm, whose performance is directly proportional to the square of the size of the input data.
        Exapmle:- Traversing a 2D array

        Others Example:-Other examples: Bubble sort, insertion sort and selection sort algorithms (we will discuss these algorithms later in separate tutorials)
        others big O notation :- logarithmic growth O(log n), log-linear growth O(n log n), exponential growth O(2^n) and factorial growth O(n!).

        The performance of an algorithum:-
        O(1) < O(log n) < O (n) < O(n log n) < O(n^2) < O (n^3)< O(2^n) < O(n!)



### 2. Omega Notation (Ω) – 
      Omega(Ω) notation specifically describes best case                       scenario

    -  Omega notation specifically describes best case scenario. It represents the lower bound running time complexity of an algorithm. So if we represent a complexity of an algorithm in Omega notation, it means that the algorithm cannot be completed in less time than this, it would at-least take the time represented by Omega notation or it can take more (when not in best case scenario).

### 3. Theta Notation (θ) – 
     This notation represents the average complexity of an algorithm.

    - This notation describes both upper bound and lower bound of an algorithm so we can say that it defines exact asymptotic behaviour. In the real case scenario the algorithm not always run on best and worst cases, the average running time lies between best and worst and can be represented by the theta notation.



## Two Pointer Algorithum
Two Pointer Technique uses two-pointer in one loop over the given data structure. It is commonly used for solving array, string, linked list coding problems.Two pointers is really an easy and effective technique which is typically used for searching pairs in a sorted array.

    
     


               
