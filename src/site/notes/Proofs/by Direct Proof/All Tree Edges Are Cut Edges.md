---
{"dg-publish":true,"permalink":"/proofs/by-direct-proof/all-tree-edges-are-cut-edges/"}
---

#### Conjecture
Conjecture 3 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]].
If $T$ is a tree, then every edge of $T$ is a cut edge.
#### Initial Thoughts
* In a tree, there is only one path between two distinct vertices.
* Removing a cut edge makes a graph disconnected.
* Trees are connected.
* Trees never contain cycles.
* Contrapositive: If an edge is not a cut edge, then it is not in a tree.
#### Proof by Direct Proof
Let $e = \{u, v\}$ be an arbitrary edge in a tree, $T$ = $(V, E)$.

By definition, trees are connected and acyclic. Also, since $T$ is a tree, there must be exactly one path between $u$ and $v$.

If there is exactly one path between $u$ and $v$, and there is an edge $e$ between $u$ and $v$, the path must be the edge $e$. If there was another path from $u$ to $v$, then the graph would be cyclic and not a tree. 

Because $e$ is the only path from $u$ to $v$, 