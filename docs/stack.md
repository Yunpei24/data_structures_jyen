# Stacks

A **stack** is a linear data structure that follows the **LIFO** (Last In First Out) principle.

## Characteristics

- Elements are added (pushed) and removed (popped) from the **top**
- Useful for undo operations, expression evaluation, and more
- Access is restricted to the top element only

## Common Operations

| Operation | Description | Time Complexity |
|-----------|-------------|----------------|
| `push()` | Add an item to the top of stack | O(1) |
| `pop()` | Remove and return the top item | O(1) |
| `peek()` | View the top item without removing it | O(1) |
| `is_empty()` | Check if the stack is empty | O(1) |

## Visual Representation

```plaintext
     ┌────┐
     │ 40 │ ← Top (Last In)
     ├────┤
     │ 30 │
     ├────┤
     │ 20 │
     ├────┤
     │ 10 │
     ├────┤
     │  5 │ ← Bottom (First In)
     └────┘
```

## Implementation

Python's `Stack` class provides methods for standard stack operations with a private list for storage.

```python
# Example usage:
stack = Stack()
stack.push(5)
stack.push(10)
element = stack.pop()  # Returns 10
```

## Applications

- Function call management (call stack)
- Expression evaluation and syntax parsing
- Undo mechanisms in text editors
- Browser history tracking
- Backtracking algorithms

## Example Notebook

👉 See [Stack Example Notebook](https://github.com/yunpei24/data_structures_jyen/blob/main/examples/stack_example.ipynb)
