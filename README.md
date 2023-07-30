# FibonacciHeap-Java

FibonacciHeapJava is a Java implementation of the Fibonacci Heap data structure. A Fibonacci Heap is an advanced data structure that supports efficient priority queue operations such as insertion, deletion, and decrease key. It is ideal for applications requiring fast heap operations.

## Features

- Fast insertions, deletions, and updates
- Efficient decrease key operation
- Potential analysis for heap efficiency
- K smallest elements retrieval from a single-tree heap

## Usage

You can include the `FibonacciHeap.java` class in your Java project and use it to implement priority queue-based algorithms efficiently.

## Example

```java
// Creating a new Fibonacci Heap
FibonacciHeap heap = new FibonacciHeap();

// Inserting elements
heap.insert(10);
heap.insert(20);
heap.insert(5);

// Retrieving the minimum element
int min = heap.findMin().getKey();

// Decreasing the key of a node
HeapNode node = heap.insert(30);
heap.decreaseKey(node, 15);

// Deleting the minimum element
heap.deleteMin();

// Melding two Fibonacci Heaps
FibonacciHeap heap2 = new FibonacciHeap();
// ... insert elements into heap2 ...
heap.meld(heap2);
