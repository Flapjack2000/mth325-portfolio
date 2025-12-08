---
{"dg-publish":true,"permalink":"/proofs/by-contrapositive/connected-graphs-with-minimal-edges-are-trees/"}
---

#### Conjecture
>Conjecture 14 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]].

>Let $G$ be a graph with $n$ vertices. If $G$ is connected and has $n − 1$ edges, then $G$ is a tree.
#### Initial Thoughts
* Trees are connected and do not contain cycles.
* Contradiction? $G$ is connected and has $n-1$ edges but isn't a tree?
	* Show that there can't actually be a cycle if $G$ has $n-1$ edges.
* Contrapositive: If $G$ is not a tree, then $G$ is not a connected graph or $G$ does not have $n-1$ edges.
#### Proof (by Contrapositive)
The contrapositive of the conjecture is this: 
>If $G$ is not a tree, then $G$ is not a connected graph or $G$ does not have $n-1$ edges.

If $G$ is not a tree and is not connected, then the contrapositive holds.

Suppose $G$ is not a tree but is connected. Because trees are connected and acyclic and $G$ is a connected non-tree, $G$ must contain a cycle.

Let $C$ be a cycle in $G$, and let $e$ be an arbitrary edge in $C$. 




**NEEDS FINISHING**

