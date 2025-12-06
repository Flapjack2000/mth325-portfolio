---
{"dg-publish":true,"permalink":"/proofs/by-contradiction/exactly-one-path-between-any-two-vertices-in-a-tree/"}
---

#### Conjecture
>Conjecture 10 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]]

>In any tree $T$, for any vertices $u$ and $v$, there is exactly one path from $u$ to $v$.
#### Initial Thoughts
* Trees are acyclic and connected graphs
* I already proved that if there are at least two distinct paths between two vertices, then there is a cycle
#### Proof (by Contradiction)
Assume for the sake of contradiction that there exists a tree $T = (V, E)$ and vertices $u, v \in V$, such that if $p$ is the number of paths from $u$ to $v$, then ${p \in {\mathbb N}} \land {p \ne 1}$. That is,  ${p = 0} \lor {p \ge 2}$. 

If $p = 0$, then $u$ and $v$ are not connected, implying that $T$ is not a connected graph. However, $T$ is a tree and must, by definition, be a connected graph. Therefore, $p \ne 0$.

If $p \ge 2$, then there are at least two distinct paths between $u$ and $v$. [[Proofs/by Direct Proof/Two Distinct Paths Between Two Vertices Imply a Cycle\|Therefore, $T$ contains a cycle]]. However, $T$ is a tree and must, by definition, be acyclic. Therefore, $p \not\geq 2$. Equivalently, $p \lt 2$.

Since ${p \in {\mathbb N}} \land ({0 \lt p \lt 2})$, the only possibility is $p = 1$, contradicting the assumption that $p \ne 1$. Therefore, there is exactly one path from $u$ to $v$.