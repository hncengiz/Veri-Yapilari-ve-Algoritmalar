#
# <center>BINARY SEARCH TREE<center>
--------------------------

#
## Working of Binary Search Tree
---------------------------------
#

Binary Search Tree is a node-based binary tree data structure which has the following properties:

- The left subtree of a node contains only nodes with keys lesser than the node’s key.
- The right subtree of a node contains only nodes with keys greater than the node’s key.
- The left and right subtree each must also be a binary search tree.


**1. Display the steps of the array [7, 5, 1, 8, 3, 6, 0, 9, 4, 2] using Binary-Search-Tree**
#

##### Step 1 :
#

Insert 7 into the tree as the node. 
#
|     Description    |  |  |  |
|--                  |- |- |- |
|     **"node"**     |  | 7|  |

#
##### Step 2 :
#
5 is lesser than 7, so it is added to the left subtree of the node.
#
|     Description  |  |  |  |
|--                |- |- |- |
|                  |  |  |7 |
|                  |  | / |  |
|   <center>**insert 5**<center> |5 |  |  |

#
##### Step 3 :
#

1 is lesser than 7 and 5, so it is added to the left subtree of 5.
#

|     Description  |  |  |  |  |  |
|--                |- |- |- |- |- |
|                  |  |  |  |  |7 |
|                  |  |  |  | / | |
|                  |  | |5 |  |  |
|                  |  |/ |  |  |  |
|   <center>**insert 1**<center> |1 | |   |  |  |

#
##### Step 4 :
#

8 is greater than 7, so it is added to the right subtree of the node.
#

|     Description  |  |  |  |  |  |  |  |
|--                |- |- |- |- |- |- |- |
|                  |  |  |  |  |7 |  |  |
|                  |  |  |  | / | |\  |  |
|   <center>**insert 8**<center>   |  |  |5 |  |  |  | 8 |
|                  |  |/ |  |  |  |  |  |
|                  | 1|  |  |  |  |  |  |
#
##### Step 5 :
#

3 is lesser than 7 and 5, greater than 1, so it is added to the right subtree of 1.
#

|     Description  |  |  |  |  |  |  |  |
|--                |- |- |- |- |- |- |- |
|                  |  |  |  |  |7 |  |  |
|                  |  |  |  | / | |\  |  |
|                  |  |  |5 |  |  |  | 8 |
|                  |  |/ |  |  |  |  |  |
|                  | 1|  |  |  |  |  |  |
|                  |  | \ |  |  |  |  |  |
|  <center>**insert 3**<center> |  |  | 3 |  |  |  |  |
#
##### Step 6 :
#

6 is lesser than 7 and greater than 5, so it is added to the right subtree of 5.
#

|     Description  |  |  |  |  |  |  |  |
|--                |- |- |- |- |- |- |- |
|                  |  |  |  |  |7 |  |  |
|                  |  |  |  | / | |\  |  |
|                  |  |  |5 |  |  |  | 8 |
|                  |  |/ |  | \ |  |  |  |
|      <center>**insert 6**<center>        | 1  |  |  |  | 6 |  |
|                  |  | \ |  |  |  |  |  |
|                  |  |  | 3 |  |  |  |  |
#
##### Step 7 :
#

0 is lesser than 7,5 and 1, so it is added to the left subtree of 1.
#

|     Description  |  |  |  |  |  |  |  |  |  |
|--                 |- |- |- |- |- |- |- |- |- |
|                   |  |  |  |  |  |  |7 |  |  |
|                   |  |  |  |  |  | / | |\  |  |
|                  |  |  |  |  |5 |  |  |  | 8 |
|                  |  |  |  |/ |  | \ |  |  |  |
|                  |  |  | 1  |  |  |  | 6 |  |
|                 |  | / |  | \ |  |  |  |  |  |
|    <center>**insert 0**<center>              | 0 |  |  |  | 3 |  |  |  |  |

#
##### Step 8 :
#

9 is greater than 7 and 8, so it is added to the right subtree of 8.
#

|     Description  |  |  |  |  |  |  |  |  |  |  |  |
|--                 |- |- |- |- |- |- |- |- |- |- |- |
|                   |  |  |  |  |  |  |7 |  |  |  |  |
|                   |  |  |  |  |  | / | |\  |  |  |  |
|                  |  |  |  |  |5 |  |  |  | 8 |  |  |
|                  |  |  |  |/ |  | \ |  |  |  | \ |  |
|       <center>**insert 9**<center>           |  |  | 1  |  |  |  | 6 |  |  |  | 9 |
|                 |  | / |  | \ |  |  |  |  |  |  |  |
|                  | 0 |  |  |  | 3 |  |  |  |  |  |  |

#
##### Step 9 :
#

4 is lesser than 7 and 5, greater than 1 and 3, so it is added to the right subtree of 3.
#

|     Description  |  |  |  |  |  |  |  |  |  |  |  |
|--                 |- |- |- |- |- |- |- |- |- |- |- |
|                   |  |  |  |  |  |  |7 |  |  |  |  |
|                   |  |  |  |  |  | / | |\  |  |  |  |
|                  |  |  |  |  |5 |  |  |  | 8 |  |  |
|                  |  |  |  |/ |  | \ |  |  |  | \ |  |
|                  |  |  | 1  |  |  |  | 6 |  |  |  | 9 |
|                 |  | / |  | \ |  |  |  |  |  |  |  |
|                  | 0 |  |  |  | 3 |  |  |  |  |  |  |
|                  |  |  |  |  |  | \ |  |  |  |  |  |
|       <center>**insert 4**<center>             |  |  |  |  |  |  | 4 |  |  |  |  |
#
##### Step 10 :
#

2 is lesser than 7, 5 and 3, greater than 1, so it is added to the left subtree of 3.
#

|     Description  |  |  |  |  |  |  |  |  |  |  |  |
|--                 |- |- |- |- |- |- |- |- |- |- |- |
|                   |  |  |  |  |  |  |7 |  |  |  |  |
|                   |  |  |  |  |  | / | |\  |  |  |  |
|                  |  |  |  |  |5 |  |  |  | 8 |  |  |
|                  |  |  |  |/ |  | \ |  |  |  | \ |  |
|                  |  |  | 1  |  |  |  | 6 |  |  |  | 9 |
|                 |  | / |  | \ |  |  |  |  |  |  |  |
|                  | 0 |  |  |  | 3 |  |  |  |  |  |  |
|                  |  |  |  | / |  | \ |  |  |  |  |  |
|       <center>**insert 2**<center>             |  |  | 2 |  |  |  | 4 |  |  |  |  |
#

**As a result, it looks like as follows;**
#

|  |  |  |  |  |  |  |  |  |  |  |
|- |- |- |- |- |- |- |- |- |- |- |
|  |  |  |  |  |  |7 |  |  |  |  |
|  |  |  |  |  | / | |\  |  |  |  |
|  |  |  |  |5 |  |  |  | 8 |  |  |
|  |  |  |/ |  | \ |  |  |  | \ |  |
|  |  | 1  |  |  |  | 6 |  |  |  | 9 |
|  | / |  | \ |  |  |  |  |  |  |  |
| 0 |  |  |  | 3 |  |  |  |  |  |  |
|  |  |  | / |  | \ |  |  |  |  |  |
|  |  | 2 |  |  |  | 4 |  |  |  |  |


#
**BST Gif**
#

![](../../../../Downloads/bst.gif.gif)

#

#### Patika Link

[patika.dev](https://app.patika.dev/tmrs)