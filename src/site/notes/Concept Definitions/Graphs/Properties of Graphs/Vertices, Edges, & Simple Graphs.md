---
{"dg-publish":true,"permalink":"/concept-definitions/graphs/properties-of-graphs/vertices-edges-and-simple-graphs/"}
---

A simple graph consists of two sets: a vertex set and an edge set.

An element of the vertex set is called a vertex or node. 
An element of the edge set is called an edge or arc. Each edge is an unordered pair of vertices. 

Thus, a graph is an ordered pair of set, $G = (V, E)$. 
$G$ is a graph with vertex set $V$ and edge set $E$.
#### Incidence & Adjacency
When vertices $v$ and $w$ are the endpoints of an edge $e$, we say that:
* Each vertex is *incident* to the edge.
* The edge is *incident* to each vertex.
* The vertices are *adjacent* to each other.

The simple graph $G$, shown below, consists of
* a vertex set $V = \{v_1, v_2, v_3, v_4, v_5, v_6, v_7, v_8,\}$
* an edge set $E = \{(v_1, v_3), (v_1, v_5), (v_2, v_5), (v_3, v_4), (v_3, v_5), (v_6, v_7), (v_6, v_8)\}$
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/disconnected-graph.png?raw=true" >
	  <figcaption><i>A graph, G.</i></figcaption>
	</figure>
</div>