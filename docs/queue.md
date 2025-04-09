# Queues

A **queue** is a linear data structure that follows the **FIFO** (First In First Out) principle.

## Characteristics

- Elements are added from the **rear** and removed from the **front**
- Used in scheduling, buffering, and task queues
- Maintains insertion order for processing

## Common Operations

| Operation | Description | Time Complexity |
|-----------|-------------|----------------|
| `enqueue()` | Add an item to the rear of the queue | O(1) |
| `dequeue()` | Remove and return the front item | O(1) |
| `peek()` | View the front item without removing it | O(1) |
| `is_empty()` | Check if the queue is empty | O(1) |

## Visual Representation

```plaintext
       enqueue                dequeue
          ↓                      ↑
        ┌────┬────┬────┬────┬────┐
Rear → │ 40 │ 30 │ 20 │ 10 │  5 │ ← Front
        └────┴────┴────┴────┴────┘
```

## Implementation

Python's `Queue` class uses a list-based implementation with operations that maintain FIFO behavior.

```python
# Example usage:
queue = Queue()
queue.enqueue(5)
queue.enqueue(10)
element = queue.dequeue()  # Returns 5
```

## Applications

- Task scheduling in operating systems
- Print job queues
- BFS (Breadth-First Search) algorithm
- Request handling in web servers
- Call center systems

## Example Notebook

👉 See [Queue Example Notebook](https://github.com/yunpei24/data_structures_jyen/blob/main/examples/queue_example.ipynb)
