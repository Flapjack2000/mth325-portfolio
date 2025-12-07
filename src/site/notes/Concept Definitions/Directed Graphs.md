---
{"dg-publish":true,"permalink":"/concept-definitions/directed-graphs/"}
---

In a *directed graph*, the edges between vertices are unidirectional. The edges of a directed graph are often depicted with arrows, rather than lines.

Directed graphs are also called *digraphs*.

Below is a directed graph, $$D = (V_D = \{v_A, v_B, v_C, v_D\}, E_D = \{(v_A, v_B), (v_A, v_C), (v_B, v_C), (v_D, v_C)\}$$ and its underlying undirected graph, $$U = (V_U = \{v_A, v_B, v_C, v_D\}, E_U = \{\{v_A, v_B\}, \{v_A, v_C\}, \{v_B, v_C\}, \{v_D, v_C\}\}.$$
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/directed-graph.png?raw=true" >
	  <figcaption><i>A directed graph, D.</i></figcaption>
	</figure>
	
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/undirected-graph.png?raw=true" >
	  <figcaption><i>An undirected graph, U.</i></figcaption>
	</figure>
</div>

Note that the edges in the edge set of a directed graph are notated as ordered pairs of vertices, rather than sets. The edge begins at the first element in the ordered pair (the tail of the edge), and ends at the second (the head of the edge).

Also, note that while $U$ contains a 3-cycle, $D$ does not. 

#### In-degree & Out-degree
Given a directed graph $G$, for any vertex $v$, the in-degree of the $v$ is the number of edges to $v$, and the out-degree of $v$ is the number of edges from $v$.

In $D$, $v_B$ has in-degree 1, which can be written as $deg^-(v_B) = 1$. $v_B$ also has out-degree 1, which can be written as $deg^+(v_B) = 1$.

