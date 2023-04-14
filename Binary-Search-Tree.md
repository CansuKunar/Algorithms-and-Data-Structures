# Binary Search Tree
### What is the Binary Search Tree? 
A Binary Search Tree is a type of tree structure where each node can have at most two child nodes, typically called the left and right child. 
Nodes to the left of a given node contain values smaller than the node, and nodes to the right contain values larger. 
This allows for efficient searching, insertion, and deletion of nodes in the tree. 
To search for a value in a Binary Search Tree, you compare the value you're searching for with the value of the current node and move left or right accordingly. 
To insert a new value, you traverse the tree in the same way as searching and add a new node at the appropriate location. 
To delete a node, you find the node to be removed, replace it with its predecessor or successor node, and remove the predecessor or successor 
node from its previous location to maintain the structure of the tree.<br>


### Binary-Search-Tree steps of the **[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]**  series.
1. Start with the root node containing the first element of the series, which is 7.
   -       7


2. Compare the next element in the series, which is 5, to the root node value. Since 5 is less than 7, we add it as the left child of the root node.
   -          7
            /
          5

3. Compare the next element, 1, to the root node value. Since 1 is less than 7, we move to the left child node. Since there is no left child node for the node containing 5, we add 1 as the left child of that node.
   -                7
                   / \
                  5   
                 /     
                1   
4. Compare the next element, 8, to the root node value. Since 8 is greater than 7, we move to the right child node. Since there is no right child node for the node containing 7, we add 8 as the right child of that node.
   -                7
                   / \
                  5   8
                 /     
                1       
5. Compare the next element, 3, to the root node value. Since 3 is less than 7, we move to the left child node. We compare 3 to the value of the node containing 5. Since 3 is less than 5, we add it as the left child of that node.
   -                7
                   / \
                  5   8
                 / \
                1   3 

6. Compare the next element, 6, to the root node value. Since 6 is greater than 7, we move to the right child node. We compare 6 to the value of the node containing 8. Since there is no left child node for that node, we add 6 as the left child of that node.
   -                7
                   / \
                  5   8
                 / \
                1   3
                     \
                      6
7. Compare the next element, 0, to the root node value. Since 0 is less than 7, we move to the left child node. We compare 0 to the value of the node containing 5. Since there is no left child node for that node, we add 0 as the left child of that node.
   -                7
                   / \
                  5   8
                 / \
                1   3
               /     \
              0       6


8. Compare the next element, 9, to the root node value. Since 9 is greater than 7, we move to the right child node. We compare 9 to the value of the node containing 8. Since there is no right child node for that node, we add 9 as the right child of that node
   -                7
                   / \
                  5   8
                 / \   \
                1   3   9
               /     \
              0       6
  
  
9. Compare the ninth element, 4, with the root node, which is less, so it becomes the right child of the left child node (3).
   -                7
                   / \
                  5   8
                 / \   \
                1   3   9
               /   / \
              0   4   6
              
10. Compare the tenth element, 2, with the root node, which is less, so it becomes the left child of the right child node (4).
   -                7
                   / \
                  5   8
                 / \   \
                1   3   9
               /   / \
              0   4   6
                 /
                2
                
                
