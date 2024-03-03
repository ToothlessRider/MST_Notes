#  DAA Notes for MST
> Author : Aaron Augustine

## Basics ( Variables, Datatypes, etc )
> Ref : [Chap_1_pdf](https://classroom.google.com/c/NjU3MzUwMzg0NDgy/m/NjU4Mjc0MDkzNDYx/details)

## Variables
X, y, z or any other alphabets that are used as "==placeholders==" to store values ( data ) are known as variables.

## Data types
The variables defined form equations when used. To solve the equations we need them to hold specific types of values and 'data type' is the name being use to define those specific values.
*In Programming language it is a set of data with values having predefined characteristics* 
> Ex. : char, integer, boolean, long int, short int, etc

There are two types of Data Types : 
- System defined data types / Primitive Data types ( ==int, float, char, double, bool, etc ....== )
- User Defined Data types : 
![](https://lh7-us.googleusercontent.com/rylKh1jPp5tTkKNDRyDw4jy8VJTXGnKO9BAdBF_AhoevlPpGEkTV8AYI693xJW3NIaByvFifQNjldUqIYLJWQmN6AXWRIQGK0S_UqY3n9AW3zUthqG20MaaMf1m636t69-LZNgKVz1k4tg9Q758DkZ4)

## Data Structure 
*Data Structure is a particular way of storinga nd organizing data on a computer so that it can be used efficiently*
There are two types of Data Structures : 
* Linear Data Structures ( *elements are accessed in a ==sequential order==*)
* Non-Linear Data Structures (*elements are stored/accessed in a ==non-linear order==*)

## Abstract Data Types ~ADT's~
When we combine the user defined data structures with their operations they are known as 'Abstract Data Types', and they consist of two parts : 
* Declaration of Data
* Declaration of Operations

Ex : Linked Lists, Stacks, Queues, Priority Queues, Binary Trees, Dictionaries, Disjoint Sets, Hash Tables, Graphs, etc

## Questions!!

>Q1. What is an Algorithm ? Why do we analyse algorithms?

Ans. *An Algorithm is the step-by-step instruction given to sove a certain problem*
Just how there are many ways to travel from a given 'City A' to 'City B', there can be multiple algorithms for a given question. 
Analysing them helps us figure out which algorithm is the most suitable and the most effective.

>Q2. What is running time anaylsis ?

Ans. It is the process of determining how processing time increases as the size of the problem ( input size ) increases. 
The following are the different types of inputs we encounter : 
* Size of an array
* Polynomial Degree
* Number of elements in a  matrix
* Number of bits in binary representation of the input
* Vertices and edges of a  graph

## Commonly Used Rate of growths

**![](https://lh7-us.googleusercontent.com/2xn1LSkl1ln_fqdyGy_zTpqf4RTOVa0sWsjRShl66SWilHgt-vIoXbMa7UWKujaJloy0GvPnxFczfhL_LzM2rTnV5uwGmueezRQlzw6egAeUFlsz7K2MmsSkXXMkPC1OOPp3U79SFFbfby5Xk-5EACE)**
The table above shows the relation between different rates of growth and examples

**![](https://lh7-us.googleusercontent.com/7lwSiL-rvYP66ye8VnLkpxkWpex5wZjH1UExrhnFXop-0t5aBDcRVLWNGWT67t9ni1An9V5__tkyLXh9RAvEKdYRlhukY0dGOtvuFlcPv2fKdPjQgDFsFCPE7DXg1l_OH6tlPA9Q5LzrCEJZHEpM4Hg)**
The flowchart above describes the decrease in time complexity, of the rate of growth.

> There are 3 types of analyis : 
> * Worst Case
> * Best Case 
> * Averge Case

##  Big-O Notation
*Represented as f(n) = O(g(n)), i.e. for larger values of n, f(n) = g(n)




<hr>

# Arrays and Linked Lists 

## Linked List 
It is a DS used to store collections of data, and it has the following properties
* Successive elements are connected by pointers.
* Last elements points to NULL
* Can grow or shrink in size during execution of a program
* Can be made just as long as required
* Does not waste memory space 

### Main linked list operations : 
* Insert : Inserts and element into the list
