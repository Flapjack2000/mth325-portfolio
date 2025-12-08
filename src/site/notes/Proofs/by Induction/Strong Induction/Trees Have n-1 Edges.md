---
{"dg-publish":true,"permalink":"/proofs/by-induction/strong-induction/trees-have-n-1-edges/"}
---

#### Conjecture
>Conjecture 9 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]] 

>If $T = (V, E)$ is a tree with $n$ vertices, then $T$ has $n-1$ edges. That is, $|E| = |V| -1$.
#### Initial Thoughts
* Trees are connected and do not contain cycles
* Trees are minimally connected
#### Proof (by Strong Induction)
##### Base Case
Let $T = (V, E)$ be a tree with exactly $1$ vertex. $T$ is simply a lone vertex with no edges, thus $|E| = 0$, and the conjecture holds for $n=1$.

##### Inductive Hypothesis
Assume any tree with $k$ vertices has exactly $k-1$ edges for some integer $k \ge 1$.

##### Inductive Step
Let $T = (V, E)$ be a tree with $n \ge 2$ vertices. Since $T$ is a tree and has at least two vertices, it is connected and its edge set must contain at least one edge.

Select an arbitrary edge $e$ and remove it from $T$. Because [[Proofs/by Direct Proof/All Tree Edges Are Cut Edges\|every edge in a tree is a cut edge]], $e$ must be a cut edge, and removing it must split $T$ into two separate connected components. Both components must also be trees because they are (individually) connected and removing an edge cannot create a cycle. 

Let $T_1 = (V_1, E_1)$ and $T_2 = (V_2, E_2)$ be the two connected components formed by removing the edge. Both $T_1$ and $T_2$ must contain one of the vertices formerly incident to $e$. 




**NEEDS FINISHING**
