
## BINARY TREE IN C LANGUAGE 

Overview

Tree in C is the non-linear(hierarchical) data structure, that consists of nodes connected by edges.

The binary tree in C is a special type of tree in which the parent node can have a maximum of two children nodes, i.e. it can have 0, 1, or 2 children node(s). The node of a binary tree in C contains three data variables to store the value of the node, the pointer(link) to the left child, and the pointer(link) to the right child.

Scope 

In this article, you will learn what is a tree in C, and what is a binary tree. We will also learn about the structure, and implementation, and will also see examples of a binary tree.
We will learn about different terminologies of a tree such as : root, parent, child, leaf, height, depth, path, etc.
In this article, we will know about the different types of binary trees.
You will see the implementation of the binary tree and how different functions are used.

Introduction

The tree in C is a non-linear data structure, i.e. The elements are not stored sequentially, and in the tree in C, they are present in levels. A binary tree in C is a data structure in which every node can have a maximum of two children nodes. Children nodes are labeled as right and left child. Each node in the binary tree contains a value and two pointers pointing to the children. The topmost node of the binary tree is called the root node and the bottom-most nodes of the binary tree are called leaf nodes. The height of a binary tree is calculated by taking the longest path between the root and the leaf node.

In the i'th level, the maximum number of nodes can be 2 raised to the power i, and the minimum number of nodes in a binary tree of height H is H+1.

The binary trees are implemented using pointers in C, usually, we create a structure that contains a data variable that is used to store the value of that node and two pointer variables(named left and right), the left pointer is used to point to the left child similarly, the right pointer is used to point to the right child of the node.

The binary tree in C can also be implemented using the array data structure. If P is the index of the parent element then the left child will be stored in their index 
(
2
�
)
+
1
(2p)+1, and the right child will be stored in the index 
(
2
�
)
+
2
(2p)+2

What are Trees in C ?
The tree is a non-linear data structure in C that contains nodes that are not connected linearly, rather they are connected in a hierarchical manner. The nodes are present at different levels and are connected by edges. Between the set of two connected nodes, the one which is at the upper level is considered a parent, and the lower one is considered a child node.

In Tree in C, a parent node can have many children nodes. The diagram below shows the structure of the tree in C.

https://scaler.com/topics/images/trees-in-c.webp

n the above image of the tree, A is the root node. B, C, and E are the children of node A, and they have 2, 1, and 2 children respectively. Here, D, G, F, H, L, K, and M are the leaf nodes.

A binary tree in C is a special case of the tree, which can have only two children nodes (left child and right child).



Tree Terminologies

various terminologies are related to the tree :

Root :

The first node of the binary tree is known as the root node of the binary tree. There cannot be any tree without a root node as it is the origin of the tree and the root node does not have any parent element. We cannot have more than one root node in a tree.

Edge :

The connecting link between the two nodes is known as the edges of the tree it is also referred to as the branch of a tree. If there are n nodes in a binary tree then there will be a total of n-1 edges.

Parent :

A node that has a connecting link to another node in the level below is known as a parent node. In a more formal term, a node that is a predecessor of another node is called a parent node.

Child :

Any node which is connected to a node that is one level above it, is known as the child node. In formal terms, it can be said that every note that is a descendant of any node is known as a child node. Every not present in the tree can be considered as a child node except the root node.

Siblings :

The children node that shares the same parent node are referred to as siblings.

Leaf :

A node with no child is known as a leaf node. It is the terminal node of the tree.

Internal Node :

The nodes that have at least one child node is known as an internal node. Every node (even the root node) is an internal node except the leaf nodes.

External Node :

A node that doesn't have any child node is considered an external node.

Ancestors :

Ancestors of a node, are the nodes in the path from the root to the current node, including the root node, and excluding the current node are ancestors of the current node.

Descendants :

Descendants of a node, are the nodes that are below its level and are also connected to it, directly or via nodes. All the children, their children, and so on are the descendants of the current node.

Path :

A path between any two nodes of a tree is the sequence of connected nodes along with the edges between the two nodes. And the path length is the number of nodes present between two nodes.

Level :

The level in the tree represents the number of steps from the top/root. The root node of the tree is said to be at level 0, and as we go downwards the level increases

Depth :

The depth of any node in the tree is the length of the path from the root node to that particular node, i.e. The number of nodes between that particular node and the root node.

Height :

The height of any node is given by the maximum number of edges from the leaf node to that particular node.

Applications of Trees

The application of trees are :

It is used where we need to create hierarchical data.
Multistage decisions making can be created using trees.

It can be used to store the data of the dictionary and can be used for fast and efficient spell-checking.

In the blockchain, a special kind of binary tree known as the Merkle tree is used, which is a binary tree of the hashes of the transactions in the blockchain.

Representation of Binary Tree in C

A binary tree can be represented using a linked list and also using an array. Representation of this tree, using both(array and linked list) is explained below.

Array Representation :
The binary tree can be represented using an array of size 2n+1 if the depth of the binary tree is n. If the parent element is at the index p, Then the left child will be stored in the index 
(
2
�
)
+
1
(2p)+1, and the right child will be stored in the index 
(
2
�
)
+
2
(2p)+2.


The array representation of the above binary tree is :
As in the above binary tree, A was the root node, so it will be stored in the 0th index. The left child of A will be stored in the 2(0)+1 that is equal to the 1st location. So, B is stored in index 1. And, similarly, the right child of A will be stored in the 2(0)+2 index. For every node, the left and right child will be stored accordingly.


