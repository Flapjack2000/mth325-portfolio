---
{"dg-publish":true,"permalink":"/concept-definitions/trees/"}
---

*Trees* are connected graphs that contain no cycles. A collection of trees is called a *forest*. Since a forest is made of one or more trees, a forest can also be described as any graph containing no cycles.

If the degree of a vertex of a tree is $1$, then it can be called a *leaf*.

A graph $T = (V, E)$ is a tree if and only if, for any distinct vertices $u, v \in V$, there is exactly one path from $u$ to $v$.

#### Rooted Trees

A *rooted tree* is a tree, $T$, with a designated vertex, $r$, called the root. 

The length of the path from the root to a vertex is called the vertex's distance from the root. All edges in the path are directed from vertices with lower distance to vertices with higher distance from the root.

Any vertex with an edge pointing toward a particular vertex is the parent of that vertex, and any vertex that has an edge pointing away from that vertex is a child of that vertex.

If two vertices share the same parent, then they are called siblings.

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/rooted-tree.png?raw=true" >
	  <figcaption><i>A rooted tree.</i></figcaption>
	</figure>
</div>

#### Binary Trees
A *binary tree* is a rooted tree
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/binary-tree.png?raw=true" >
	  <figcaption><i>A binary tree.</i></figcaption>
	</figure>
</div>