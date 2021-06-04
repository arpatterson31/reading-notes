# Class Reading: Graphs

## Vocab terms

- **Vertex:** also called a node, it is a data object that can have zero or more adjacent vertices

- **Edge:** connection between two nodes

- **Neighbor:** node adjacent of another node, connected via an edge

- **Degree:** number of edges connected to a vertex

## Types of Graphs

### Undirected

A graph where each edge is undirected or bi-directional. It does not move in any direction.

### Directed

A graph where every edge is directed. Each node is directed to another node with a specific requirement of what node should be referenced next.

### Complete

A graph with all nodes connected to all other nodes

### Connected

A graph that has all nodes having at least one edge

### Disconnected

A graph where some nodes might not have edges (poor little lonely nodes...out on an island by itself)

### Acyclic

A directed graph without cycles
*cycle:* node can be traversed through and potentially end up back at itself

### Cyclic

A directed graph with cycles

## Traversal

Traversal is similar to trees (Breadth First & Depth first)

- Breadth first is similar to trees but watch out if the graphs have cycles because that can send you in an infinite loop!
- You need to keep track if you have visited a node to avoid this

## Real world use case

- Netflix uses graphs for suggestions!
