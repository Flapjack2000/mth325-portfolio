---
{"dg-publish":true,"permalink":"/concept-definitions/trees/"}
---

*Trees* are connected graphs that contain no cycles. A collection of trees is called a *forest*. Since a forest is made of one or more trees, a forest can also be described as any graph containing no cycles.

If the degree of a vertex of a tree is $1$, then it can be called a *leaf*.

A graph $T = (V, E)$ is a tree if and only if, for any distinct vertices $u, v \in V$, there is exactly one path from $u$ to $v$.

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/tree(1).png?raw=true" >
	  <figcaption><i>A tree.</i></figcaption>
	</figure>
</div>

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/forest.png?raw=true" >
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/forest(1).png?raw=true" >
	  <figcaption><i>Two forests.</i></figcaption>
	</figure>
</div>

#### Rooted Trees
A *rooted tree* is a tree, $T$, with a designated vertex, $r$, called the root. 

The length of the path from the root to a vertex is called the vertex's distance from the root. All edges in the path are directed from vertices with lower distance to vertices with higher distance from the root.

Any vertex with an edge pointing toward a particular vertex is the parent of that vertex, and any vertex that has an edge pointing away from that vertex is a child of that vertex.

If two vertices share the same parent, then they are called siblings.

In $R$, the rooted tree shown below, the vertex $C$ has three children, namely $H$, $I$, and $J$. The vertex $A$ is the root of $R$ and is an *ancestor* of all other vertices in the tree because there is a path from $A$ to any other vertex in the tree and $A$ has a lower distance from the root than any other vertex (a distance of $0$ to be exact). The vertex $F$ is a *descendent* of the vertices $D$, $B$, and $A$ because there is a path from those vertices to $F$ and $F$ has a higher distance from the root of the tree than those vertices.

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/rooted-tree.png?raw=true" >
	  <figcaption><i>A rooted tree, R.</i></figcaption>
	</figure>
</div>

#### Binary Trees
A *binary tree* is a rooted tree for which every vertex has at most $2$ children.
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/binary-tree.png?raw=true" >
	  <figcaption><i>A binary tree.</i></figcaption>
	</figure>
</div>