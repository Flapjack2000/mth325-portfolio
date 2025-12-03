---
{"dg-publish":true,"permalink":"/proofs/by-direct-proof/two-distinct-paths-between-two-vertices-imply-a-cycle/"}
---

#### Conjecture
* Conjecture 1 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]].
In a graph $G$, if there are at least $2$ distinct paths from a vertex $u$ to another vertex $v$, then $G$ contains a cycle.
#### Initial Thoughts
* If you have two different paths from $u$ to $v$, the paths must split at some point and rejoin later, making a cycle.
#### Proof (by Direct Proof)
Let $G=(V, E)$ be a graph with vertices $u, v \in V$. Between $u$ and $v$, there are at least $2$ distinct paths.

Let $P_1 = [x_0, x_1, ..., x_k]$ and $P_2 = [y_0, y_1, ..., y_m]$ be any two distinct paths from $u$ to $v$.