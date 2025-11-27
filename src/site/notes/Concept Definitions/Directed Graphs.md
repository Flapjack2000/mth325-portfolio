---
{"dg-publish":true,"permalink":"/concept-definitions/directed-graphs/"}
---

In a *directed graph*, the edges between vertices are unidirectional. The edges of a directed graph are often depicted with arrows, rather than lines.

Directed graphs are also called digraphs.

Below is a directed graph, $$D = (V_D = \{A, B, C, D\}, E_D = \{(A, B), (A, C), (B, C), (D, C)\}$$ and its underlying undirected graph, $$G = (V_G = \{A, B, C, D\}, E_G = \{\{A, B\}, \{A, C\}, \{B, C\}, \{D, C\}\}.$$
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/directed-graph.png?raw=true" >
	  <figcaption><i>A directed graph, D.</i></figcaption>
	</figure>
	
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/undirected-graph.png?raw=true" >
	  <figcaption><i>An undirected graph, G.</i></figcaption>
	</figure>
</div>

Note that the edges in the edge set of a directed graph are notated as ordered pairs, rather than sets. The edge begins at the first element in the ordered pair, and ends at the second.

Also, note that while $G$ contains a cycle, $D$ does not. 

#### In-degree & Out-degree
