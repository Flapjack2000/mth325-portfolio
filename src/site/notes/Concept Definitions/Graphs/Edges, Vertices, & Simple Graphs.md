---
{"dg-publish":true,"permalink":"/concept-definitions/graphs/edges-vertices-and-simple-graphs/"}
---

A simple graph consists of two sets: a vertex set and an edge set.

An element of the vertex set is called a vertex or node. 
An element of the edge set is called an edge or arc. Each edge is an unordered pair of vertices. 

Thus, a graph is an ordered pair of set, $G = (V, E)$. 
$G$ is a graph with vertex set $V$ and edge set $E$.

#### Incidence & Adjacency
When vertices $v$ and $w$ are the endpoints of an edge $e$, we say that:
* Each vertex is *incident* to the edge.
* The edge is *incident* to each vertex.
* The vertices are *adjacent* to each other.

The number of edges incident to a vertex is called the *degree* of the vertex. For a single, isolated vertex, its degree is $0$.