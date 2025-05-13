# Ex14 Heap Tree
## DATE:1/5/2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1.Start
2.Find the index of the element num in the array.
3.Swap the element to be deleted with the last element in the array. 
4.Decrease the array size (size) by 1. 5.Start heapifying from the last non-leaf node (index size/2 - 1). 
6.Call heapify() to restore the heap property for each node. 
7.End

## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: SRIKAAVYAA T
RegisterNumber: 212223230214
*/

struct n { 
char d; 
struct n *l; 
struct n *r; 
};
void preOrder(struct n *tree) 
{ 
if(tree) 
{ 
printf("%c",tree->d); 
preOrder(tree->l); 
preOrder(tree->r); 
} 
} 
void inOrder(struct n *tree) 
{ 
if(tree) 
{ 
inOrder(tree->l); 
printf("%c",tree->d); 
inOrder(tree->r); 
} 
} 
void postOrder(struct n *tree) 
  
  
{ 
if(tree) 
{ 
postOrder(tree->l); 
postOrder(tree->r); 
printf("%c",tree->d); 
} 
} 
```

## Output:
![image](https://github.com/user-attachments/assets/e717ad2b-0dc5-4cef-a2c3-2734f3519151)



## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
