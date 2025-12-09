---
{"dg-publish":true,"permalink":"/proofs/by-contrapositive/if-an-edge-is-the-only-path-between-its-endpoints-it-s-a-cut-edge/"}
---


#### Conjecture
>Conjecture 2 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]]

>In a connected graph, $G$, if an edge $(u,v)$ is the only path from $u$ to $v$, then $(u,v)$ is a cut edge. 

#### Initial Thoughts
* Definition of cut edge: If an edge in a connected graph would leave a subgraph that is not connected if it were deleted, then that edge is a *cut edge*.

#### Proof (by Contrapositive)
The contrapositive of the conjecture is this:
> Let $G = (V, E)$ be a connected graph, and let $e = (u, v)$ be an arbitrary edge in $E$ between vertices $u$ and $v$. If $e$ is not a cut edge, then there exists another path from $u$ to $v$ that does not contain $(u, v)$.

Suppose $e$ is not a cut edge. By definition, removing a cut edge from a graph would result in a subgraph that is disconnected. Therefore, if $e$ is not a cut edge, removing it must not result in a subgraph that is disconnected. That is, $G$ must remain connected if $e$ is removed.

Since $G - e$ is connected, there must be a path between every pair of vertices in the graph, including another path between $u$ and $v$ that does not include $e$. 

Therefore, the contrapositive holds, and the original conjecture is proven.