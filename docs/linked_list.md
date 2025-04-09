# Linked List

A Linked List is a linear data structure where elements are stored in separate memory locations and connected through references (pointers).

## Features

- **Dynamic Size**: Unlike arrays, linked lists can grow or shrink at runtime
- **Efficient Insertions/Deletions**: Adding or removing elements doesn't require shifting other elements
- **No Random Access**: Elements must be accessed sequentially from the first node
- **Extra Memory**: Requires additional memory for storing references/pointers

## Types of Linked Lists

1. **Singly Linked List**: Each node points to the next node
2. **Doubly Linked List**: Each node points to both next and previous nodes
3. **Circular Linked List**: Last node points back to the first node

## Visual Representation

```plaintext
Singly Linked List:
┌─────┬─────┐    ┌─────┬─────┐    ┌─────┬─────┐
│ A   │  ●──┼────▶ B   │  ●──┼────▶ C   │ null│
└─────┴─────┘    └─────┴─────┘    └─────┴─────┘
 data  next       data  next       data  next
```

## Implementation

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

class LinkedList:
    def __init__(self):
        self.head = None
    
    def append(self, data):
        new_node = Node(data)
        if not self.head:
            self.head = new_node
            return
        
        current = self.head
        while current.next:
            current = current.next
        current.next = new_node
```

## Time Complexity

| Operation | Time Complexity |
|-----------|----------------|
| Access    | O(n)           |
| Search    | O(n)           |
| Insertion | O(1)*          |
| Deletion  | O(1)*          |

\* When position is known, otherwise O(n) to find the position first

## Example

Check the [Linked List Notebook](https://github.com/yunpei24/data_structures_jyen/blob/main/examples/linked_list_example.ipynb) for implementation details.

---

*Note: Unlike arrays, linked lists do not have fast index-based access or static size. They excel at dynamic memory allocation and efficient insertions/deletions.*
