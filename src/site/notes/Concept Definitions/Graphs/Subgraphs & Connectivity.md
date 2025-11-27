---
{"dg-publish":true,"permalink":"/concept-definitions/graphs/subgraphs-and-connectivity/"}
---

#### Subgraphs
A subgraph is a graph whose vertex and edge sets are subsets of another graph's vertex and edge sets. To denote that a graph $G'$ is a subgraph of the graph $G$, we would write $G' \subseteq G$

Suppose we have two graphs, $A = (V_A, E_A)$ and $B = (V_B, E_B)$.
$$(V_B \subseteq V_A) \land (E_B \subseteq E_A) \implies B \subseteq A$$
#### Connected Components
A connected component is a maximal group of vertices in a graph where there is a path between any two vertices in the group. It is a maximally connected subgraph.

The graph $G$, shown below, has two connected components.

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/disconnected-graph.png?raw=true" >
	  <figcaption><i>A graph, G, with two connected components.</i></figcaption>
	</figure>
</div>