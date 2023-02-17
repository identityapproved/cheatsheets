---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience
---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience
Created: 17.02.2023 15:45
Links:
___

### Arrays vs Linked List

Lets contrast these

-   Usability:
	- Array: 
			1. Idexing accessing
			2. Can't insert value into an array without writing the for loops manually to shift averything over, and put in your value, or unshift.
	- LinkedList:
			1. Traverse each item in list until find. => always linear search
-   Time: 
	- Array => O(1)
-   Space:
	- Array => should allocate all memory upfront
	- LL => create node with links (use less memory)

### Array List 
(or dynamic array)

![[arraylist.excalidraw]]

get -> O(1)
push/pop -> O(1)
un/shift -> O(N)

### Ring Buffer
- in Rust -> VecDeque (double ended ring buffer)

![[ringbuffer.excalidraw]]

(log batching, object pooling)

```ad-hint
Everithing needs to be O(1), if possible.
```
