

# <center> MERGE SORT <center>
-------------------------------

#

## Working of Merge Sort Algorithm
------------------------------------

Merge sort is a divide and conquer algorithm. It divides input array in two halves, calls itself for the two halves and then merges the two sorted halves.

- Two functions are involved in this algorithm 
    - The merge function is used for merging two halves.
    - The Merge sort function recursively calls itself to divide the array till size becomes one.
#
**1. Show how to sort the array {16,21,11,8,12,22} using merge sort**
#

##### Step 1:
#
-  Divide the array into two parts,
-  Divide these two arrays into further parts,
-  Divide the array until further division is not possible,
#
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|-----------------------------------------------  |- |- |- |- |- |- |- |- |- |- |- |- |
|1.|  |  |  |16|21|11|8 |12|22|  |  |  |
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|2. |  |  |16|21|11|  |  |8 |12|22|  |  |
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|3.|  |16|21|  |11|  |  |8 |  |12|22|  |
|                                                 |  |  |  |  |  |  |  |  |  |  |  |  |
|4.                                                 |16|  |21|  |11|  |  |8 |  |12|  |22|

#
##### Step 2:
#
- After dividing the array into smallest units, merging starts based on comparison of elements,
- Firstly, compare the element for each list and then combine them into another list in a sorted manner.
#

|  |  |  |  |  |  |  |  |  |  |  |  |  |
|----------------------------------------------- |- |- |- |- |- |- |- |- |- |- |- |- |
|     |16|  |21|  |11|  |  |8 |  |12|  |22|
|  |  |  |  |  |  |  |  |  |  |  |  |  |
|5.|  |16|21|  |11|  |  |8 |  |12|22|  |
|                                                |  |  |  |  |  |  |  |  |  |  |  |  |
|6. |  |  |11|16|21|  |  |8 |12|22|  |  |
|                                                |  |  |  |  |  |  |  |  |  |  |  |  |
|7.       |  |  |  |8 |11|12|16|21|22|  |  |  |

#

**As a result, it looks like as follows;**
#
# 
![](../../../../Desktop/merge%20sort.png)

#
#
**2. Big-O Notation of the Array**
###
O( n * (logn) ) --> O( 6 * (log6) )

#

### Patika Link

[patika.dev](https://app.patika.dev/tmrs)


