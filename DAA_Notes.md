#  DAA Notes for MST
> Author : Aaron Augustine

> Star the gist so that I can get a consensus on how many people are using this resource

# Sorting Algorithms

> Cheat sheet for algorithm Time Complexity 

| Algorithm | Best | Average | Worst |
|--|--|--|--|
| Binary Search | O(1) | O(logn) | O(logn) |
|Selection Sort|O(N^2^) | O(N^2^) | O(N^2^)|
| Quick Sort | O(nlogn) | O(nlogn) | O(N^2^) |
|Merge Sort | O(nlogn) | O(nlogn) | O(nlogn) |
|Insertion Sort & Bubble Sort | O(n) | O(N^2^)|O(N^2^)|
|Unsorted Case| O(1) | O(n) | O(n) |

<hr>

> [Additional Reference : GFG Sorting Techniques](https://www.geeksforgeeks.org/analysis-of-different-sorting-techniques/)


## Unsorted Case  

*Best Case* : Here the best case would be if the element to be found is the first element [ O(1)]
*Average Case* : O(n)
*Worst Case* : Element to be found is the last element [ O(n) ] 

#### *Algorithm*
```
function search(A, K)
    i = 0;

    while i < n and A[i] != K do
        i = i + 1;

    if i < n
        return i;
    else
        return -1;

```
#### *Python Code*
```python
def search(array, k ):
	i = 0
	n = len(array)
while i < n and A[i] != k : 
	i = i + 1

if i <n : 
	return i;
else : 
	return -1;

#remaining code to input the values into unsorted search
```

> Worst case would be the need to scan the entire sequence A. 
> * Time complexity : O(n)

**Now let us look at the case where A is sorted**
Steps to follow : 
* Compare k with midpoint of A
* If midpoint is K, the value is found
* If K < midpoint, search left half of the array
* If K > midpoint, search right half of the array

## Binary Search 
*Best Case* : Here the best case would be if the element to be found is the middle element [ O(1)]
*Average Case* : O(log~2~n)
*Worst Case* : Element to be found is the last element [ O(log~2~n) ] 

> Since it is **Binary** search, the base of the log will be 2

#### *Algorithm*
```
bsearch(K, A, l, r) // A sorted, search for K in A[l..r-1]
    if (r - l == 0)
        return false

    mid = (l + r) div 2 // integer division

    if (K == A[mid])
        return true

    if (K < A[mid])
        return bsearch(K, A, l, mid)
    else
        return bsearch(K, A, mid + 1, r)
```


#### *Python Code*
```python
def bsearch(k, array, l, r) :
	if ( r - l == 0):
		return false
	
	mid = ( l + r )/2
	if ( k == arra[mid]) : 
		return true
	if ( k < array[mid]):
		return (bsearch(k, array, l, mid))
	else:
		return (bsearch(k, array, mid+1, r))

#remaining code to input the values into bsearch
```

> T(n) : time to search an array of size n :
> T(0) = 1
> T(n) = 1 + T(n/2)

Therefore if we unwind the recurrence
> T(n) = 1 + 1 + T(n/2^2^) = .....
> T(n) = 1 + 1 + ...... + T(n/2^k^)
> T(n) = 1 + 1 + ... + 1 + T(n/2^logn^) = O(logn)

**Binary search works only for arrays**

## Selection Sort 
The idea here is to move the item into it's correct place in the final sorted list ( Not to use another extra array )

#### *Algorithm*
```
SelectionSort(A, n) // Sort A of size n
    for (startpos = 0; startpos < n; startpos++)
        // Scan segments A[0]..A[n-1], A[1]..A[n-1], ...
        
        minpos = startpos;
        for (i = minpos + 1; i < n; i++)
            if (A[i] < A[minpos])
                minpos = i;

        swap(A, startpos, minpos)

```

#### *Java Code*

```java
import java.io.*;
import java.util.Scanner;

public class selection_sort {
    
    void sort(int arr[]) {
        int n = arr.length;

        // Traversing the array
        for(int i = 0; i < n; i++) {
            int min_idx = i;
            for(int j = i + 1; j < n; j++) {
                if(arr[j] < arr[min_idx])
                    min_idx = j;
            }

            // Time to swap them
            int temp = arr[min_idx];
            arr[min_idx] = arr[i];
            arr[i] = temp;
        }
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        selection_sort ob = new selection_sort();

        // int arr[] = {24, 70, 22, 4, 65, 7, 21};
        System.out.print("Input the size of the array to be sorted : ");
        int size = scanner.nextInt();

        int arr[] = new int[size];

        System.out.print("Input the elements of the array : ");
        for(int i = 0; i < size; i++) {
            arr[i] = scanner.nextInt();
        }

        scanner.close();

        ob.sort(arr);
        System.out.println("Sorted Array");
        int n = arr.length;
        for(int i = 0; i < n; i++) {
            System.out.print(arr[i] + " ");
            System.out.println();
        }
    }
}

```

> Time complexity : O(n^2^)
> Finding minimum in unsorted segment of length k requires one scan, k steps
> T(n) = n + (n-1) + (n-2) + ..... + 1 = n(n+1)/2 = O(n^2^)

## Selection Sort ~Recursive~

#### *Algorithm*
```
SelectionSort(A, start, n) // Sort A from start to n-1
    if (start >= n - 1)
        return;

    // Locate minimum element and move to start of segment
    minpos = start;
    for (i = start + 1; i < n; i++)
        if (A[i] < A[minpos])
            minpos = i;

    swap(A, start, minpos)

    // Recursively sort the rest
    SelectionSort(A, start + 1, n)

```

#### *Python Code*
```python
def selection_sort_recursive(A, start, n):
    if start >= n - 1:
        return
    
    # Locate minimum element and move to start of segment
    minpos = start
    for i in range(start + 1, n):
        if A[i] < A[minpos]:
            minpos = i
    
    # Swap elements
    A[start], A[minpos] = A[minpos], A[start]
    
    # Recursively sort the rest
    selection_sort_recursive(A, start + 1, n)

# Example usage:
array = [64, 25, 12, 22, 11]
selection_sort_recursive(array, 0, len(array))

print("Sorted array:", array)

```



# Questions for MST

>Q1. What is an Algorithm ? Why do we analyse algorithms?

Ans. *An Algorithm is the step-by-step instruction given to sove a certain problem*
Just how there are many ways to travel from a given 'City A' to 'City B', there can be multiple algorithms for a given question. 
Analysing them helps us figure out which algorithm is the most suitable and the most effective.

<hr>

>Q2. What is running time anaylsis ?

Ans. It is the process of determining how processing time increases as the size of the problem ( input size ) increases. 
The following are the different types of inputs we encounter : 
* Size of an array
* Polynomial Degree
* Number of elements in a  matrix
* Number of bits in binary representation of the input
* Vertices and edges of a  graph

<hr>

> Q3. 

# Introduction PPT - Shortnotes


## Basics ( Variables, Datatypes, etc )
> Ref : [Chap_1_pdf](https://classroom.google.com/c/NjU3MzUwMzg0NDgy/m/NjU4Mjc0MDkzNDYx/details)

## Variables
X, y, z or any other alphabets that are used as "*placeholders*" to store values ( data ) are known as variables.

## Data types
The variables defined form equations when used. To solve the equations we need them to hold specific types of values and 'data type' is the name being use to define those specific values.
*In Programming language it is a set of data with values having predefined characteristics* 
> Ex. : char, integer, boolean, long int, short int, etc

There are two types of Data Types : 
- System defined data types / Primitive Data types ( *int, float, char, double, bool, etc ....* )
- User Defined Data types : 
![](https://lh7-us.googleusercontent.com/rylKh1jPp5tTkKNDRyDw4jy8VJTXGnKO9BAdBF_AhoevlPpGEkTV8AYI693xJW3NIaByvFifQNjldUqIYLJWQmN6AXWRIQGK0S_UqY3n9AW3zUthqG20MaaMf1m636t69-LZNgKVz1k4tg9Q758DkZ4)

## Data Structure 

> [Reference : Data structure based mcqs](https://www.sanfoundry.com/sorting-multiple-choice-questions-mcq/)


*Data Structure is a particular way of storinga nd organizing data on a computer so that it can be used efficiently*
There are two types of Data Structures : 
* Linear Data Structures ( *elements are accessed in a sequential order*)
* Non-Linear Data Structures (*elements are stored/accessed in a non-linear order*)

## Abstract Data Types ~ADT's~
When we combine the user defined data structures with their operations they are known as 'Abstract Data Types', and they consist of two parts : 
* Declaration of Data
* Declaration of Operations

Ex : Linked Lists, Stacks, Queues, Priority Queues, Binary Trees, Dictionaries, Disjoint Sets, Hash Tables, Graphs, etc


## Commonly Used Rate of growths

**![](https://lh7-us.googleusercontent.com/2xn1LSkl1ln_fqdyGy_zTpqf4RTOVa0sWsjRShl66SWilHgt-vIoXbMa7UWKujaJloy0GvPnxFczfhL_LzM2rTnV5uwGmueezRQlzw6egAeUFlsz7K2MmsSkXXMkPC1OOPp3U79SFFbfby5Xk-5EACE)**
The table above shows the relation between different rates of growth and examples

**![](https://lh7-us.googleusercontent.com/7lwSiL-rvYP66ye8VnLkpxkWpex5wZjH1UExrhnFXop-0t5aBDcRVLWNGWT67t9ni1An9V5__tkyLXh9RAvEKdYRlhukY0dGOtvuFlcPv2fKdPjQgDFsFCPE7DXg1l_OH6tlPA9Q5LzrCEJZHEpM4Hg)**
The flowchart above describes the decrease in time complexity, of the rate of growth.

> There are 3 types of analyis : 
> * Worst Case
> * Best Case 
> * Averge Case

## Asymptotic Notation
[Reference : Aysmptotic notations - Big-O,Ω and theta](https://www.youtube.com/watch?v=A03oI0znAoc)


##  Big-O Notation 
*This shows upper bound of a function
*Represented as f(n) = O(g(n)), i.e. for larger values of n, f(n) = g(n)


## Big-Ω Notation
* This shows lower bound of a function



## Theta Notation
* This shows the average bound of afunction
<hr>

# Arrays and Linked Lists 
> [Reference : Array and Array ops mcqs](https://www.sanfoundry.com/data-structure-questions-answers-array-array-operations/)

## Linked List 
It is a DS used to store collections of data, and it has the following properties
* Successive elements are connected by pointers.
* Last elements points to NULL
* Can grow or shrink in size during execution of a program
* Can be made just as long as required
* Does not waste memory space 

### Main linked list operations : 
* **Insert** : Inserts an element into the list
* **Delete** : Deletes an element from the list : 

### Auxillary linked list operations
* **Delete List** : Removes all the elements of the list / disposes of the list 
* **Count** : Returns the number of elements in the list 
* Find n^th^ node from the end of the list

<hr>

## Arrays 
**![](https://lh7-us.googleusercontent.com/u1tT-MC3ilPz4B14Z2NyewoKneBuAs41xufwguVhYx6IxN7KlHDKjs_dQOzdfMnpiQOQxgySPUvwLUH8dH_z7XApN1KkeJRDNGB37wRtLl1jQvv9FY3TBTzKOYWC3wO4wQSt5FNPDuPy1asdyXZj5_4)**

### Advantages of Arrays : 
1. Simple and easy to use 
2. Faster access to the elements

### Disadvantages of Arrays : 
1. **Fixed Size** : The size of the array is static ( specify the array size before using it ) 
2.**One block allocation** : To allocate the array at the beginning itself, sometimes it may not be possible to get the memory for the complete array.
3. **Complex position-based insertion** : TO insert an element at a given position we may need to shift the elements. This will create a position for us to insert the new element at the desired position.

**The main disadvantage of linked lists is the long access time for any element in a linked list**

## Difference between Linked Lists and Arrays
**![](https://lh7-us.googleusercontent.com/NAA1UFQ0FDQeuqWy0qmLmAL3aa8nVEAc7xyeI33P_7z_wl6LB-HX0YPwEFI0Ul3mlQscFeqcspIVXxbLGESJcB6eb4I3dLwD8-16mUQPMTdd8XUI9H8NBzPXFhLimice1EWISd3OotRYumeAUyyi28g)**


# Stacks and Queues

## Stacks
A stack is a simple data structure used for storing data. In this the order that they arrive in is important, just like a stack of plates, the first one stacked is the last to be used.

> Two operations that can be done on astack are "Push" (insert data ) and "Pop" ( remove data )

**![](https://lh7-us.googleusercontent.com/eB8AtQSRUY1d89s7QtMfoSSsiVcKzPgAbnwL6hhH5-EJyjPV77aE7FMjnH1QGBbiJluc-malu0khGY975dkPQyWkYZgZTEJwpv1m9Yk_DB32auUOUPxUCTVRtz38hemQMRklcb4frrTUsXEKywRM89Q)**



# Searching and Sorting 

> [Reference : Sorting based mcqs](https://www.sanfoundry.com/sorting-multiple-choice-questions-mcq/)
> 

