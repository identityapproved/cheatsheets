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