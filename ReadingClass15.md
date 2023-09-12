# Title: Exploring the Tree Data Structure

# WHY Study Trees?

The tree data structure is crucial in computer science for organizing and managing data efficiently. It provides a hierarchical model that is widely used in various applications.

# WHAT is a Tree?

A tree is a collection of nodes organized in a hierarchical manner. It starts with a single node known as the root, which can have zero or more child nodes. Each node may have its own child nodes, creating a branching structure.

# HOW does a Tree Work?

Root Node: This is the starting point of the tree and serves as the root of all subsequent nodes.
Child Nodes: These are nodes that branch out from a parent node. They form the next level of the hierarchy.
Leaves: These are nodes that do not have any children. They are at the ends of the branches.
Parent Nodes: Each node (except the root) has a parent, which is the node it directly stems from.
Siblings: Nodes that share the same parent are considered siblings.
Detail: Tree Terminology

Root: The topmost node with no parent.
Parent: A node that has one or more child nodes.
Child: A node that is a direct descendant of another node.
Leaf: A node with no children.
Siblings: Nodes that share the same parent.

# Visualization:

       A
      / \
     B   C
    / \
D   E

# A vocabulary/definition list
Tree: A hierarchical data structure consisting of nodes connected by edges. It starts with a single node called the root and branches out into child nodes.

Node: A fundamental unit in a tree that contains a value and may have zero or more child nodes.

Root: The topmost node in a tree. It has no parent and serves as the starting point for traversing the tree.

Parent: A node that has one or more child nodes originating from it.

Child: A node that is a direct descendant of another node.

Leaf: A node in a tree with no children. It is located at the ends of the branches.

Siblings: Nodes that share the same parent node.

Depth: The level or distance of a node from the root. The root node is at depth 0.

Height: The maximum depth of a tree, i.e., the longest path from the root to a leaf.

Binary Tree: A tree in which each node has at most two children, typically referred to as the left child and right child.

Binary Search Tree (BST): A type of binary tree where the left child of a node contains values less than or equal to the node's value, and the right child contains values greater than the node's value.

Traversal: The process of visiting and processing each node in a tree in a specific order.
In-Order Traversal: A depth-first traversal that starts from the left subtree, visits the left child, then the root, and finally the right child.

Pre-Order Traversal: A depth-first traversal that starts from the root, then visits the left subtree, and finally the right subtree.

Post-Order Traversal: A depth-first traversal that starts from the left subtree, then visits the right subtree, and finally the root.

Breadth-First Traversal (Level Order Traversal): A traversal that explores all nodes at the current depth before moving on to nodes at the next depth level.

Balanced Tree: A tree where the height of the left and right subtrees of any node differ by at most one.

Unbalanced Tree: A tree where the height of the left and right subtrees of a node can differ significantly.

Complete Binary Tree: A binary tree in which every level, except possibly the last, is completely filled, and all nodes are as left as possible.

Full Binary Tree: A binary tree in which every node has either 0 or 2 children.

Perfect Binary Tree: A binary tree in which all interior nodes have exactly two children and all leaf nodes are at the same level.



