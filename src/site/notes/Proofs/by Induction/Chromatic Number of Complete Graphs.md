---
{"dg-publish":true,"permalink":"/proofs/by-induction/chromatic-number-of-complete-graphs/"}
---


#### Conjecture
For every integer $n \ge 1$, the chromatic number $X(n)$ of the complete graph $K_n$ is exactly $n$.
#### Initial Thoughts
* In a complete graph, every vertex is adjacent to every other vertex.
* If you add a vertex to a complete graph, it must use a new color because it is adjacent to every other vertex.
#### Proof (by Induction)
**Base Case**
The complete graph $K_1$ has only one vertex, so it requires only one color. Thus, $X(K_1) = 1$, and the conjecture holds true.

**Inductive Hypothesis**
Assume that for some integer $k \ge 1$, the chromatic number of the complete graph $K_k$ is $k$. Each vertex in $K_k$ has a unique color assigned to it.

**Inductive Step**
The complete graph  $K_{k+1}$ can be created by adding a vertex to $K_k$ and connecting that vertex to every other vertex with a new edge. 

$K_{k+1}$ can be colored by assigning 
* color $1$ to $v_1$,
* color $2$ to $v_2$,
* color $3$ to $v_3$,
* . . .,
* color k to $v_k$, 
* and color $k+1$ to $v_{k+1}$.

This is a valid coloring using $k+1$ colors, so $X(K_{k+1})$.