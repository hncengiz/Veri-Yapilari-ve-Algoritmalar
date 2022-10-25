# <center> INSERTION SORT <center>
------------------------------------


## Working of Insertion Sort Algorithm
-------------------------------------
#
- Select the first unsorted element,
- Swap other elements to the right to create the correct position and shift the unsorted element,
- Advance the marker to the right one element.

#
####  <span style="color: red"> 1. Show how to sort the array {22,27,16,2,18,6} using insertion sort </span>
---------------------------------------------------------------------------------------------------------------
#

<style>
    .heatMap {
        width: 70%;
        }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
        text-align: center;

</style>

<div class="heatMap">

 | 22 | 27 | 16 | 2 | 18 | 6 | 
 |----|----|----|---|----|---| 

#

##### Step 1: 
#

Initially, the sorted sub-array contains the first element in the array. Insert 27 into the sub-array.
#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
    }

</style>

  
 | 22 | 27 | 16 | 2 | 18 | 6 | 
 |----|----|----|---|----|---|

#
##### Step 2: 
#
The sorted sub-array is {22, 27}. Insert 16 into the sub-array.
#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
    }

</style>

  
 | 16 | 22 | 27 | 2 | 18 | 6 | 
 |----|----|----|---|----|---| 

#
##### Step 3: 
#
The sorted sub-array is {16, 22, 27}. Insert 2 into the sub-array.
#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
    }

</style>

  
 | 2 | 16 | 22 | 27 | 18 | 6 | 
 |----|----|----|---|----|---| 
#
 ##### Step 4:
#
The sorted sub-array is {2, 16, 22, 27,}. Insert 18 into the sub-array.
#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
    }

</style>

  
 | 2 | 16 | 18 | 22 | 27 | 6 | 
 |----|----|----|---|----|---|

#
##### Step 5: 
#
The sorted sub-array is {2, 16, 18, 22, 27}. Insert 6 into the sub-array.
#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
    }

</style>

  
 | 2 | 6 | 16 | 18 | 22 | 27 | 
 |----|----|----|---|----|---| 

#
##### Step 6: 
#
The entire array is now sorted.
#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgreen;
        word-wrap: break-word;
    }

</style>

  
 | 2 | 6 | 16 | 18 | 22 | 27 | 
 |----|----|----|---|----|---| 

#
####  <span style="color: red"> Big-O Notation of the Array </span>
---------------------------------------------------
#

( n - 1) + ( n - 2 ) + ( n + 3) + ... + 1 = ( n * ( n - 1 ) ) / 2 

= n ^ 2

#
####  <span style="color: red"> Which Case Contain Element 18 After The Array is Sorted? </span>
--------------------------------------------------------
#
Avarege case since element '18' is found in the middle of the array after sorting.

#
### Gif Link 
#

![insert sorting](https://user-images.githubusercontent.com/116035329/197865998-994edda2-1d4c-4ebf-8297-a1cb86047ecd.gif)


#
####  <span style="color: red"> 2. Show how to sort the first four step of the array { 7, 3, 5, 8, 2, 9, 4, 15, 6 } using insertion sort </span>
------------------------------------------------------
#

<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightgblue;
        word-wrap: break-word;
    }

</style>

  
 | 7 | 3 | 5 | 8 | 2 | 9 | 4 | 15 | 6 | 
 |---|---|---|---|---|---|---|----|---| 

#
##### Step 1: 
#

Initially, the sorted sub-array contains the first element in the array. Insert 3 into the sub-array.

#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightblue;
        word-wrap: break-word;
    }

</style>

  
 | 3 | 7 | 5 | 8 | 2 | 9 | 4 | 15 | 6 | 
 |---|---|---|---|---|---|---|----|---| 

#
##### Step 2: 
#

The sorted sub-array is {3, 7}. Insert 5 into the sub-array.

#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightblue;
        word-wrap: break-word;
    }

</style>

  
 | 3 | 5 | 7 | 8 | 2 | 9 | 4 | 15 | 6 | 
 |---|---|---|---|---|---|---|----|---|

#
##### Step 3: 
#
The sorted sub-array is {3, 5, 7}. Insert 8 into the sub-array. No need to swap.

#
<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightblue;
        word-wrap: break-word;
    }

</style>

  
 | 3 | 5 | 7 | 8 | 2 | 9 | 4 | 15 | 6 | 
 |---|---|---|---|---|---|---|----|---|

#
 ##### Step 4: 
#

The sorted sub-array is {3, 5, 7,8}. Insert 2 into the sub-array.
#

<style>
    .heatMap {
        width: 70%;
    }
    .heatMap th {
        background: lightblue;
    }

</style>

  
 | 2 | 3 | 5 | 7 | 8 | 9 | 4 | 15 | 6 | 
 |---|---|---|---|---|---|---|----|---|

#

 ## Patika Link

 [patika.dev](https://app.patika.dev/tmrs)
