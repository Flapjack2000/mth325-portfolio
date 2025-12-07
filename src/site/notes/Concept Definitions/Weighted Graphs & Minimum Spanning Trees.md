---
{"dg-publish":true,"permalink":"/concept-definitions/weighted-graphs-and-minimum-spanning-trees/"}
---

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/weighted-directed-graph.png?raw=true" >
	  <figcaption><i>A weighted directed graph.</i></figcaption>
	</figure>
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/weighted-undirected-graph.png?raw=true" >
	  <figcaption><i>A weighted undirected graph.</i></figcaption>
	</figure>
</div>

A *weighted graph* is a graph where each edge is assigned a value, which is called its weight. Weights can represent just about anything: cost, profit, capacity, distance, time, strength, energy, etc.

#### Minimum Spanning Trees
A minimum spanning tree (or MST) is a subgraph of a connected, weighted graph that connects all vertices with the minimum possible total edge weight. 

It's possible for a weighted graph to have multiple MSTs. For example, imagine a complete graph with every edge assigned the same weight. 

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/weighted-graph.png?raw=true" >
	  <figcaption><i>A weighted graph, G.</i></figcaption>
	</figure>
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/mst.png?raw=true" >
	  <figcaption><i>The minimum spanning tree of G.</i></figcaption>
	</figure>
</div>