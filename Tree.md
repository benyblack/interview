# Tree
**Tree** represents the nodes connected by edges. Two famous type of trees are BinaryTree and BinarySearchTree.
**Binary Tree** is a special datastructure used for data storage purposes. A binary tree has a special condition that each node can have a maximum of two children. A binary tree has the benefits of both an ordered array and a linked list as search is as quick as in a sorted array and insertion or deletion operation are as fast as in linked list. ([source](https://www.tutorialspoint.com/data_structures_algorithms/tree_data_structure.htm))
A **Binary Search Tree** (BST) is a tree in which all the nodes follow the below-mentioned properties.
 - The left sub-tree of a node has a key less than or equal to its parent node's key.
 - The right sub-tree of a node has a key greater than to its parent node's key.
 ([source](https://www.tutorialspoint.com/data_structures_algorithms/binary_search_tree.htm))

 ## Complexity for BST
 - Access: O(log n) => worse case O(n)
 - Search: O(log n) => worse case O(n)
 - Insert: O(log n) => worse case O(n)
 - Delete: O(log n) => worse case O(n)
 - Space: O(n log(n))
