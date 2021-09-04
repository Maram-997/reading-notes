# Read 15 - Trees :
## Trees : 
 a tree is a widely used abstract data type that simulates a hierarchical tree structure, with a root value and subtrees of children with a parent node, represented as a set of linked nodes.
A tree data structure can be defined recursively as a collection of nodes (starting at a root node), where each node is a data structure consisting of a value, together with a list of references to nodes (the "children"), with the constraints that no reference is duplicated, and none points to the root.
![img](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5f/Tree_%28computer_science%29.svg/220px-Tree_%28computer_science%29.svg.png)
## Traversals : 
An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:
1. **Depth First**
Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal:

Pre-order: root >> left >> right
In-order: left >> root >> right
Post-order: left >> right >> root
![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png)
>our traversals would result in different paths:
>Pre-order: A, B, D, E, C, F
>In-order: D, B, E, A, F, C
>Post-order: D, E, B, F, C, A

2. **Breadth First**
Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. So, given our starting tree one more time:
![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/tree-example.png)
>Our output using breadth first traversal is now:
>Output: A, B, C, D, E, F

## Binary Tree Vs K-ary Trees:
In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

## K-ary Trees :
If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.
 #### Breadth First Traversal 
 Traversing a K-ary tree requires a similar approach to the breadth first traversal. We are still pushing nodes into a queue, but we are now moving down a list of children of length k, instead of checking for the presence of a left and a right child.
![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/KaryTree1.png)
>If we traversed this tree Breadth First we should see the output:
>Output: A, B, C, D, E, F, G, H

## Big O of Adding a node :
The Big O time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n). Because of the lack of organizational structure in a Binary Tree, the worst case for most operations will involve traversing the entire tree. If we assume that a tree has n nodes, then in the worst case we will have to look at n items, hence the O(n) complexity.
The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree. For example, in the above tree, w is 4.

## Binary Search Trees :
A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.
**Searching a BST**
![img](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BST2.PNG)
Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.
Let’s say we are searching 15. We start by comparing the value 15 to the value of the root, 23.
15 < 23, so we traverse the left side of the tree. We then treat 8 as our new “root” to compare against.
15 > 8, so we traverse the right side. 16 is our new root.
15 < 16, so we traverse the left side. And aha! 15 is our new root and also a match with what we were searching for.
> The best way to approach a BST search is with a while loop. We cycle through the while loop until we hit a leaf, or until we reach a match with what we’re searching for.

#### Big O of a Binary Search Tree’s :
The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n.

The Big O space complexity of a BST search would be O(1). During a search, we are not allocating any additional space.