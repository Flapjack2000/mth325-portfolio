---
{"dg-publish":true,"permalink":"/proofs/by-contrapositive/connected-graphs-with-minimal-edges-are-trees/"}
---

#### Conjecture
>Conjecture 14 from [[Proofs/Dr. Wells' List of Conjectures\|Dr. Wells' List of Conjectures]].

>Let $G$ be a graph with $n$ vertices. If $G$ is connected and has $n − 1$ edges, then G is a [[Concept Definitions/Trees\|tree]].
#### Initial Thoughts
* Trees are connected and do not contain cycles.
* Contradiction? $G$ is connected and has $n-1$ edges but isn't a tree?
	* Show that there can't actually be a cycle if $G$ has $n-1$ edges.
#### Proof (by Contrapositive)
Let $G$ be a connected graph with $n$ vertices. 

The contrapositive of the conjecture is this: 
* If $G$ is not a tree, then $G$ does not have $n-1$ edges.
