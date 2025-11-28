---
{"dg-publish":true,"permalink":"/proofs/all-tree-edges-are-cut-edges/"}
---

#### Conjecture
If $T$ is a tree, then every edge of $T$ is a cut edge.
#### Initial Thoughts
* In a tree, there is only one path between two distinct vertices.
* Removing a cut edge makes a graph disconnected.
* Trees are connected.
* Trees never contain cycles.
* Contrapositive: If an edge is not a cut edge, then it is not in a tree.
#### Proof by Direct Proof
Let $e = \{u, v\}$ be an edge in a tree, $T$ = $(V, E)$.

By definition, trees are connected and acyclic. Because $T$ is a tree, there must be exactly one path between $u$ and $v$.