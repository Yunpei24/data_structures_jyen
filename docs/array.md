# Arrays

Arrays are fundamental data structures used to store elements in **contiguous memory locations**.

## Characteristics

- Fast index-based access (constant time)
- Static size (fixed at creation time)
- Elements must be of the same type (in many languages)
- Memory efficient for random access operations

## Common Operations

| Operation | Description | Time Complexity |
|-----------|-------------|----------------|
| Access | Retrieve element at index | O(1) |
| Insert | Add element at specific position | O(n) |
| Delete | Remove element at specific position | O(n) |
| Search | Find element by value | O(n) |
| Update | Change value at specified index | O(1) |

## Visual Representation

```plaintext
┌────┬────┬────┬────┬────┐
│ 10 │ 20 │ 30 │ 40 │ 50 │
└────┴────┴────┴────┴────┘
  0    1    2    3    4    ← Indices
```

## Implementation

Python's `Array` class provides an implementation with fixed capacity and common array operations.

```python
# Example usage:
arr = Array(5)  # Create array with capacity 5
arr.insert_at(0, 10)
arr.insert_at(1, 20)
element = arr.get(0)  # Returns 10
```

## Applications

- Storing and accessing sequential data
- Matrix operations
- Lookup tables and hash tables
- Image processing
- Buffer implementations

## Example Notebook

👉 See [Array Example Notebook](https://github.com/yunpei24/data_structures_jyen/blob/main/examples/array_example.ipynb)
