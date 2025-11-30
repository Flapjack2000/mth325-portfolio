---
{"dg-publish":true,"permalink":"/proofs/by-induction/chromatic-number-of-complete-graphs/"}
---


#### Conjecture
For every integer $n \ge 1$, the chromatic number $X(K_n)$ of the complete graph $K_n$ is exactly $n$.
#### Initial Thoughts
* In a complete graph, every vertex is adjacent to every other vertex.
* If you add a vertex to a complete graph, it must use a new color because it is adjacent to every other vertex.
#### Proof (by Induction)
**Base Case**
The complete graph $K_1$ has only one vertex, so it requires only one color. Thus, $X(K_1) = 1$, and the conjecture holds true.

**Inductive Hypothesis**
Assume that for some integer $k \ge 1$, the chromatic number of the complete graph $K_k$ is $k$. Each vertex in $K_k$ has a unique color assigned to it.

**Inductive Step**
The complete graph $K_{k+1}$ can be created by adding a vertex to $K_k$ and creating an edge between that vertex and every other vertex.

To color $K_{k+1}$, the same $k$ colors from $K_k$ can be used, plus a new color $k+1$. Therefore, $X(K_{k+1}) \le k+1$.

Because $K_{k+1}$ is a complete graph, the new $(k+1)$-th vertex, $v_{k+1}$, is adjacent to each of the other $k$ vertices, so $v_{k+1}$ must be assigned a color that isn't used in $K_k$. Therefore, $X(K_{k+1}) \ge k+1$.

Since $K_{k+1}$ can be colored with $k+1$ colors and cannot be colored with fewer than $k+1$ colors, $X(K_{k+1}) = k+1$.