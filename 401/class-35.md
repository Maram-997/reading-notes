# Read - 35 : Graphs

## Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

## Terminology used when working with Graphs

1. Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. Edge - An edge is a connection between two nodes.
3. Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
4. Degree - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

* Undirected Graphs
An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
* A Directed Graph also called a Digraph is a graph where every edge is directed.

>Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

![img](https://www.alberton.info/images/articles/graphs/graphs_directed_undirected.png)

## Complete vs Connected vs Disconnected

* Complete Graphs
A complete graph is when all nodes are connected to all other nodes.
* Connected Graphs
A connected graph is graph that has all of vertices/nodes have at least one edge.
* Disconnected Graphs
A disconnected graph is a graph where some vertices may not have edges.

![img](https://i0.wp.com/algorithms.tutorialhorizon.com/files/2019/10/Connected-Undirected-Graph-Example.png?resize=967%2C397&ssl=1)

## Acyclic vs CyclicAcyclic graphs

* Acyclic Graph
An acyclic graph is a directed graph without cycles.
A cycle is when a node can be traversed through and potentially end up back at itself.
* Cyclic Graphs
A Cyclic graph is a graph that has cycles.
A cycle is defined as a path of a positive length that starts and ends at the same vertex.

![img](https://www.researchgate.net/profile/Elisa-Bertino/publication/2431833/figure/fig2/AS:339592545882121@1457976580886/Example-of-cyclic-and-acyclic-graphs.png)

## Graph Representation

We represent graphs through:

1. Adjacency Matrix
An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix
Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection
2. Adjacency List
An adjacency list is the most common way to represent graphs.
An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.
Adjacency lists make it easy to view if one vertices connects to another.

![img](https://algorithmtutor.com/images/graph_representation_directed.png)

## Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.

![img](https://s3.amazonaws.com/learneroo-images/main/Weighted-Graph-Matrix.png)

## Traversals

You will be required to traverse through a graph. The traversals itself are like those of trees. Below is a breakdown of how you would traverse a graph.

### Breadth First

In a breadth first traversal, you are starting at a specific vertex/node. This node must be specified when calling the BreadthFirst() method. The breadth-first traversal of a graph is like that of a tree, with the exception that graphs can have cycles. Traversing a graph that has cycles will result in an infinite loop….this is bad. To prevent such behavior, we need to have some way to keep track of whether a vertex has been “visited” before. Upon each visit, we’ll add the previously-unvisited vertex to a visited set, so we know not to visit it again as traversal continues.

* Here is what the algorithm breadth first traversal looks like:

1. Enqueue the declared start node into the Queue.
2. Create a loop that will run while the node still has nodes present.
3. Dequeue the first node from the queue
4. if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

### Depth First

In a depth first traversal, we approach it a bit different than the way we do when working with a depth first traversal of a tree. Similar to how the breadth-first uses a queue, we are going to use a Stack for our depth-first traversal.

* The algorithm for a depth first traversal is as follows:

1. Push the root node into the stack
2. Start a while loop while the stack is not empty
3. Peek at the top node in the stack
4. If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
5. If the top node does not have any unvisited children, Pop that node off the stack
6. repeat until the stack is empty.

## Real World Uses of Graphs

Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

1. GPS and Mapping
2. Driving Directions
3. Social Networks
4. Airline Traffic
5. Netflix uses graphs for suggestions of products
