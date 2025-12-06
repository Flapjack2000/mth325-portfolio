---
{"dg-publish":true,"permalink":"/proofs/by-direct-proof/trees-with-at-least-two-vertices-have-leaves/"}
---

#### Conjecture
>Conjecture 11 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]]

>Every tree with 2 or more vertices has leaves.

#### Initial Thoughts
* Leaves are vertices with degree 1
* Trees are connected and acylic graphs
* Vertices in trees must have one path between them
#### Proof (by Direct Proof)
Let $T  = (V, E)$ be a tree with $n = |V| \ge 2$ vertices. 

Choose an arbitrary vertex $v_0 \in V$. 

Begin with the path $p = [v_0]$. Starting from $v_0$, choose an adjacent vertex $v_{i+1}$ that is not in $p$ and add it to $p$. Continue this process until it is no longer possible to move to a new adjacent vertex that is not in the path.

Once the process ends, $p=[v_0, v_1, v_2, ..., v_k]$.

The vertex $v_k$ must be adjacent to $v_{k-1}$, because that is the vertex used to reach it. Also, $v_k$ must have no other adjacent vertices, otherwise the process would not have terminated at $v_k$. 

Therefore, $v_k$ has exactly one adjacent vertex, meaning $v_k$ is a leaf.

Therefore, $T$ contains a leaf.