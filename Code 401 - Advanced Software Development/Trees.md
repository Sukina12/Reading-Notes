# Trees Summary :

##### A Tree node :  is a component which may contain it’s own values, and references to other nodes.

##### The root : is the node at the beginning of the tree.

##### K :  the maximum number of children any node may have in the tree.

![image1](https://miro.medium.com/max/606/1*wAsNx2NFmGE6OcG2Obl-8Q.jpeg)

##### Traversing a tree allows us to search for a node, print out the contents of a tree, and much more .
  *  Two Catagories :
    1. Depth First : is where we prioritize going through the depth (height) of the tree first
    2. Breadth First: Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. 

 ![image2](https://miro.medium.com/max/1838/1*VM84VPcCQe0gSy44l9S5yA.jpeg)

##### Binary Tree Vs K-ary Trees :
  * Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

  
  * There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows.

![image3](https://miro.medium.com/max/1134/1*S9O9sNJQkfwFbtaji9e25w.png)

  * K-ary Trees : If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

![image4](http://theoryofprogramming.azurewebsites.net/wp-content/uploads/2018/01/n-ary-tree-1.jpg)


##### Pseudocode : 
  * This process is very similar to our binary tree traversal, but now we check a list of children instead of a left and right child properties.

##### Adding a node:
  * "for adding a new node to a binary tree is to fill all “child” spots from the top down. To do so, we would leverage the use of breadth first traversal. During the traversal, we find the first node that does not have all it’s children filled, and insert the new node as a child. We fill the child slots from left to right".

##### Big O :
  * The Big O time complexity for inserting a new node is O(n).
  * Searching for a specific node is O(n)
  * The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree.

##### Binary Tree : 
  * The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height).

##### Sources:
[source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)


