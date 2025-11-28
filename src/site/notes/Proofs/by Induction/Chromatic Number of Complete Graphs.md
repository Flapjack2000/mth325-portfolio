---
{"dg-publish":true,"permalink":"/proofs/by-induction/chromatic-number-of-complete-graphs/"}
---


#### Conjecture
For every integer $n \ge 1$, the chromatic number $X(n)$ of the complete graph $K_n$ is exactly $n$.
#### Initial Thoughts
* In a complete graph, every vertex is adjacent to every other vertex.

#### Proof by Induction
**Base Case**
* The complete graph $K_1$ has only one vertex, so it requires only one color. Thus, $X(K_1) = 1$.

**Inductive Hypothesis**
* Assume that for some integer $k \ge 1$, the chromatic number of the complete graph $K_k$ is $k$.

**Inductive Step**
* The graph $K_k+1$ can be created by adding a vertex to $K_k$.