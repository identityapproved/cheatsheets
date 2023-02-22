---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience
---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience
Created: 16.02.2023 15:55
Links: 
- [sorting](https://theprimeagen.github.io/fem-algos/lessons/our-second-algorithms/sort)
___

### Bubble sorting

![[bubblesort.excalidraw]] => O(N^2)

#### So what sucks about an Array?

-   Deletion (zeroes writin)
-   Insertion (replacing => write)
-   Its ungrowable

### Linked List

![[linkedlist.excalidraw]]

API:
```typescript
interface LinkedList<T> { 
	get length(): number; 
	insertAt(item: T, index: number): void;
	remove(item: T): T | undefined; 
	removeAt(index: number): T | undefined;
	append(item: T): void; 
	prepend(item: T): void; 
	get(index: number): T | undefined; 
}
```

### Queue
- linear data structure that follows the First in, First Out Principle (FIFO).

![[queue.excalidraw]]

-   enqueue
-   deque
-   peek (ability to see what is first element without popping it off).

### Stack 
- linear data structure that follows the principle of Last In First Out, the opposite of a queue, a stack. In a stack, the last element inserted inside the stack is removed first.
- focusing on single pointer -> head

![[stack.excalidraw]]

```ad-info
Property access on an object in JS may or may not be constant time.
```


### QuickSort

- an algorithm that uses a _divide and conquer_ technique. The algorithm picks a pivot element and rearranges the array so elements smaller than the pivot element move to the left side of the pivot, and elements greater move to the right side. The algorithm then recursively sorts the subarrays on the left and right of the pivot element.

![[quicksort.excalidraw]]