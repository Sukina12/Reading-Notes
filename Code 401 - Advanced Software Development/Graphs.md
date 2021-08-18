# Graphs Summary :

### Defenition :
  * "A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges".

### Used terminology :
  1. Vertex : "also called a “node”, is a data object that can have zero or more adjacent vertices".
  2. Edge : "a connection between two node".
  3. Neighbor : "are its adjacent nodes, i.e., are connected via an edge".
  4. Degree : "the number of edges connected to that vertex".

### Undirected Graphs:
  * "An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction".

  ![imahe3](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

### Directed Graphs:
  * "A Directed Graph also called a Digraph is a graph where every edge is directed".
  * "Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next".

  ![image4](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

### Complete vs Connected vs Disconnected :

  * Complete Graphs :A complete graph is when all nodes are connected to all other nodes.

  * Connected :A connected graph is graph that has all of vertices/nodes have at least one edge.

  * Disconnected :A disconnected graph is a graph where some vertices may not have edges.

### Acyclic vs Cyclic :

  * Acyclic Graph :An acyclic graph is a directed graph without cycles.
     A cycle is when a node can be traversed through and potentially end up back at itself.

  * Cyclic Graphs :A Cyclic graph is a graph that has cycles.
     A cycle is defined as a path of a positive length that starts and ends at the same vertex.

### Graph Representation :
  1. Adjacency Matrix
    ![image1](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjMatrix.PNG)
  2. Adjacency List
    ![image2](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjList.PNG)

### Weighted Graphs :
  * A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.

### Traversals :
  * Breadth First : 
      1. Enqueue the declared start node into the Queue.
      2. Create a loop that will run while the node still has nodes present.
      3. Dequeue the first node from the queue
      4. if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

![image5](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/BreadthFirst.PNG)

   * Depth First:
      1. Push the root node into the stack
      2. Start a while loop while the stack is not empty
      3. Peek at the top node in the stack
      4. If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
      5. If the top node does not have any unvisited children, Pop that node off the stack
      6. repeat until the stack is empty.

  ![image7](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/Depth1.PNG)

### Real World Uses of Graphs :
  * Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:
     1. GPS and Mapping
     2. Driving Directions
     3. Social Networks
     4. Airline Traffic
     5. Netflix uses graphs for suggestions of products


