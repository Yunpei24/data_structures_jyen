# Trees

A **tree** is a hierarchical data structure with nodes connected in parent-child relationships.

## Characteristics

- The topmost node is called the **root**
- Each node can have multiple children
- Used in file systems, databases, compilers, etc.
- No cycles (unlike graphs)
- Every node (except root) has exactly one parent

## Types

| Tree Type | Description |
|-----------|-------------|
| Binary Tree | Each node has at most two children |
| Binary Search Tree (BST) | Left child < parent < right child |
| AVL Tree | Self-balancing BST |
| Red-Black Tree | Self-balancing BST with color properties |
| B-Tree | Self-balancing tree optimized for storage systems |
| Heap | Complete binary tree with heap property |

## Visual Representation

```plaintext
        ┌───┐
        │ 8 │        ← Root
        └─┬─┘
     ┌────┴────┐
   ┌─┴─┐     ┌─┴─┐
   │ 3 │     │ 10│
   └─┬─┘     └─┬─┘
  ┌──┴──┐      └──┐
┌─┴─┐ ┌─┴─┐    ┌─┴─┐
│ 1 │ │ 6 │    │ 14│
└───┘ └───┘    └───┘
```

## Common Operations

| Operation | Description | Time Complexity (BST) |
|-----------|-------------|----------------------|
| `insert()` | Add a new node | O(log n) average, O(n) worst |
| `delete()` | Remove a node | O(log n) average, O(n) worst |
| `search()` | Find a node | O(log n) average, O(n) worst |
| `traverse()` | Visit all nodes | O(n) |

## Traversal Methods

- **Preorder**: Root → Left → Right
- **Inorder**: Left → Root → Right (gives sorted output for BST)
- **Postorder**: Left → Right → Root

## Applications

- File systems organization
- Database indexing
- Decision trees in machine learning
- Expression evaluation
- Network routing algorithms

## Example Notebook

👉 See [Tree Example Notebook](https://github.com/yunpei24/data_structures_jyen/blob/main/examples/tree_example.ipynb)
