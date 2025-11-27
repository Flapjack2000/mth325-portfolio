---
{"dg-publish":true,"permalink":"/concept-definitions/graphs/properties-of-graphs/degrees-and-degree-sequences/"}
---

The number of edges incident to a vertex is called the *degree* of the vertex. For a single, isolated vertex, its degree is $0$.

* The minimum degree of a graph $G$, the smallest of all its vertex degrees, is denoted $\delta(G)$. 
* The maximum degree of a graph $G$, the largest of all its vertex degrees, is denoted $\Delta(G)$. 

The degree sequence of a graph is the list of all its vertex degrees written in *non-increasing order*.

If $Seq(G) = [d_1, d_2, ..., d_n]$, then
* $\Delta(G) = d_1$
* $\delta(G) = d_n$

The degree sequence of a graph is an isomorphic invariant. For any two graphs, if the graphs are isomorphic, then their degree sequences are the same.

The vertex degrees of $G_1$, shown below, are as follows:

$$deg(v_1) = 3$$
$$deg(v_2) = 2$$
$$deg(v_3) = 4$$
$$deg(v_4) = 1$$
$$deg(v_5) = 2$$
The degree sequence of $G_1$, $Seq(G_1) = [4, 3, 2, 2, 1]$.
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center; ">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/degree-seq-graph.png?raw=true" >
	  <figcaption><i>G<sub>1</sub></i></figcaption>
	</figure>
</div>

<hr>

To determine if there exists a simple graph that corresponds to a given degree sequence, one can use the [[Algorithms/Hakimi-Havel\|Hakimi-Havel]] algorithm