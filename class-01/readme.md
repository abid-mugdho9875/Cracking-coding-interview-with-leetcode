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
     


               
