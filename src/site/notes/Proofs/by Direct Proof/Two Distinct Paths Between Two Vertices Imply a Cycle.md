---
{"dg-publish":true,"permalink":"/proofs/by-direct-proof/two-distinct-paths-between-two-vertices-imply-a-cycle/"}
---

#### Conjecture
* Conjecture 1 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]].

>In a graph $G$, if there are at least $2$ distinct paths from a vertex $u$ to another vertex $v$, then $G$ contains a cycle.
#### Initial Thoughts
* If you have two different paths from $u$ to $v$, the paths must split at some point and rejoin later, making a cycle.
#### Proof (by Direct Proof)
Let $G=(V, E)$ be a graph with vertices $u, v \in V$. Between $u$ and $v$, there are at least $2$ distinct paths.

Let $P_1 = [x_0, x_1, ...,x_{k-1}, x_k]$ and $P_2 = [y_0, y_1, ...,y_{m-1}, y_m]$ be any two distinct paths from $u$ to $v$. 

$P_1$ and $P_2$ may share vertices other than $u$ and $v$, but because they are distinct paths, they must diverge at least once, either at $u$ or afterward. $P_1$ and $P_2$ must also converge at least once, either at $v$ or beforehand.

Let $s \in P_1 \cap P_2$ be the vertex from which the paths $P_1$ and $P_2$ diverge. Let $t \in P_1 \cap P_2$ be the vertex where the paths $P_1$ and $P_2$ reconverge for the first time.

Let $P_1'$ be the subpath of $P_1$ from $s$ to $t$, and let $P_2'$ be the subpath of $P_2$ from $s$ to $t$. A cycle can be constructed by following $P_1'$ from $s$ to $t$, then following $P_2'$ backwards from $t$ to $s$.

Therefore, $G$ is guaranteed to contain a cycle.
