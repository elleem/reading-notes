## Trees

#### Things I Want to Know More About




#### Binary Trees, Binary Search Trees, and K-ary Trees Cheat Sheet

##### Common Terminology

Node: A component of a tree which may contain its own values and references to other nodes.

Root: The first node of a tree.

K: A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k=2.

Left: A reference to one child node in a binary tree.

Right: A reference to the other child node in a binary tree.

Edge: The link between a parent and child node in a tree.

Leaf: A node that does not have any children.

Height: The number of edges from the root to the furthest leaf in a tree.

##### Traversals

Traversing a tree allows us to search for a node, print out the contents of a tree, and much more!

There are two categories of traversals when it comes to trees: Depth First and Breadth First.

##### Depth First Traversals:

Depth first traversal is where we prioritize going through the depth (height) of the tree first.

There are three methods for depth first traversal:
1. Pre-order: root >> left >> right
2. In-order: left >> root >> right
3. Post-order: left >> right >> root

##### Pre-Order Traversal:

The root is looked at first, and then the left subtree is traversed, followed by the right subtree.

##### In-Order Traversal:

The left subtree is traversed first, then the root, and finally the right subtree.

##### Post-Order Traversal:

The left subtree is traversed first, then the right subtree, and finally the root.