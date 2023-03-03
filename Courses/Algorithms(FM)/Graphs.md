---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience
---
Tags: #algorithms/typescript #course/chapter
Medium: #algorithms #computerscience 
Created: 01.03.2023 14:45
Links:
___


#### Graph Terms

_cycle_ - When you start at Node(x), follow the links, and end back at Node(x)  
_acyclic_ - A graph that contains no cycles  
_connected_ - When every node has a path to another node
_directed_ - When there is a direction to the connections. Think Twitter  
_undirected_ - !directed. Think Facebook (i haven't been on in 10 years, it may have changed)  
_weighted_ -  The edges have a weight associated with them. Think Maps  
_dag_ - Directed, acyclic graph.  


#### Implementation Terms

_node_ - a point or vertex on the graph  
_edge_ - the connection between two nodes  


#### Big O

BigO is commonly stated in terms of `V` and `E` where `V` stands for vertices and `E` stands for edges.
So `O(V * E)` means that we will check every vertex, and on every vertex we check every edge

### Adjacency List & Adj. Matrix

![[graph.excalidraw]]

![[adjmatrixsearching.excalidraw]]

```ad-summary
title: DFS Graph List RT
O(V+E)
```

### Dijkstra shortest path

Get the lowest or nearest unseen node, or unvisited node (source) -> find closest possible node to the sourse -> keep on getting the lowest distance node and then trying to update all the other distances based on this new lowest path we found.

![[dijkstrashortestpath.excalidraw]]

