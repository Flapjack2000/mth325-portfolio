---
{"dg-publish":true,"permalink":"/concept-definitions/networks-and-flows/"}
---

#### Networks
A *network* is a directed graph, $D = (V, E)$, with a *source node*, which is in-degree zero, a *terminal node* (or sink), which has out-degree zero, and a capacity, which is a function $b : E \to \mathbb Z^+$ that assigns a positive integer value to each edge.

<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/network.png?raw=true" >
	  <figcaption><i>A network with source 0 and sink 5.</i></figcaption>
	</figure>
</div>


#### Flow
A network flow is a function on a directed graph that assigns a value to each edge that is constrained by the edges' capacities. The flow originates at the source and terminates at the sink. At every vertex (except the source and sink), the total flow entering must equal the total flow leaving. The value of a flow is the total amount entering the sink.

#### Network Cut
A network cut is a way of dividing a flow network into two parts, one of which contains the source, and the other contains the sink.