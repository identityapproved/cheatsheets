---
Tags: 
Medium: #algorithms #computerscience
---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience
Created: 11.02.2023 10:10
Links: 
- [big-O](https://theprimeagen.github.io/fem-algos/lessons/algorithms-and-time-space-complexity/time-and-space-complexity)
___

### Important concepts

1.  growth is with respect to the input
2.  Constants are dropped
3.  Worst case is _usually_ the way we measure

### Array Data Structure

```node
> const a = new ArrayBuffer(6)
undefined
> a
ArrayBuffer { [Uint8Contents]: <00 00 00 00 00 00>, byteLength: 6 }
> const a8 = new Uint8Array(a)
undefined
> a8[0] = 46
46
> a
ArrayBuffer { [Uint8Contents]: <2e 00 00 00 00 00>, byteLength: 6 }
> a8[2] = 46
46
> a
ArrayBuffer { [Uint8Contents]: <2e 00 2e 00 00 00>, byteLength: 6 }
> const a16 = new Uint16Array(a)
undefined
> a16[2] = 0x2323
8995
> a
ArrayBuffer { [Uint8Contents]: <2e 00 2e 00 23 23>, byteLength: 6 }
> a16
Uint16Array(3) [ 46, 46, 8995 ]
```

```node
Uncaught RangeError: byte length of Uint16Array should be a multiple of 2 at new Uint16Array (<anonymous>)
```

- incertion at specific index => overwrites it
- deletions => set to 00

```ad-important
title: Arrays
- are fixed size, contiguous memory chunks.
```

### ![[ArrayDataStructure]]