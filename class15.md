
###  Binary Trees, Binary Search Trees, and K-ary Trees

Common Terminology:

- Node: A component in a tree that contains its own values and references to other nodes.
- Root: The initial node at the top of the tree.
- K: A number representing the maximum number of children a node can have in a K-ary tree. For binary trees, k = 2.
- Left: A reference to the left child node in a binary tree.
- Right: A reference to the right child node in a binary tree.
- Edge: The link between a parent and child node.
- Leaf: A node without any children.
- Height: The number of edges from the root to the furthest leaf in a tree.

Traversals:
- Traversing a tree allows us to search for a node, print its contents, and perform various other operations. There are two main categories of tree traversals:

1. Depth First Traversal:
This approach prioritizes exploring the depth or height of the tree first. There are three common methods for depth first traversal:

a. Pre-order: Visit the root node first, then the left child, and finally the right child.
b. In-order: Visit the left child, then the root node, and finally the right child.
c. Post-order: Visit the left child, then the right child, and finally the root node.

2. Breadth First Traversal:
This method iterates through the tree level by level, visiting each node in a breadth-first manner.

Binary Tree vs. K-ary Trees:
Binary trees allow at most two children per node, whereas K-ary trees can have more than two children. Binary trees have no specific sorting order for nodes, and nodes can be added anywhere in the tree. In contrast, binary search trees (a type of binary tree) have a specific structure where nodes smaller than the root are placed to the left, and nodes larger than the root are placed to the right. K-ary trees accommodate any number of children per node, up to the maximum specified by K.

Traversal Implementations:

1. Pre-order Traversal (Root, Left, Right):

- Output the root's value.
- If the root has a left child, recursively perform pre-order traversal on the left child.
- If the root has a right child, recursively perform pre-order traversal on the right child.

2. In-order Traversal (Left, Root, Right):

- If the root has a left child, recursively perform in-order traversal on the left child.
- Output the root's value.
- If the root has a right child, recursively perform in-order traversal on the right child.

3. Post-order Traversal (Left, Right, Root):

- If the root has a left child, recursively perform post-order traversal on the left child.
- If the root has a right child, recursively perform post-order traversal on the right child.
- Output the root's value.

Breadth First Traversal:
To perform breadth first traversal:

- Enqueue the root node.
- While the queue is not empty:
   - Dequeue the front node.
   - Output the value of the front node.
    - Enqueue any children of the front node.
Adding a Node:
In binary trees, nodes can be added anywhere, while in binary search trees, nodes are inserted in a specific order. To add a node to a binary tree, you