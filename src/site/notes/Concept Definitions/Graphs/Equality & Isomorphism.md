---
{"dg-publish":true,"permalink":"/concept-definitions/graphs/equality-and-isomorphism/"}
---

#### Graph Equality
If two graphs are *equal*, $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$, then $V_1 = V_2$ and $E_1 = E_2$.

Sometimes it can be hard to tell if two graphs are equal simply by looking at their representations because the same graph can be represented in multiple ways.

The following graphs look very different, but are, in fact, the same graph.

<div style="display:flex">
	<figure style="width:50%; text-align:center">
	  <img src="/Images/equal-graph.png" >
	  <figcaption><i>G<sub>1</sub></i></figcaption>
	</figure>

	<figure style="width:50%; text-align:center">
	  <img src="/Images/equal-graph(1).png" >
	  <figcaption><i>G<sub>2</sub></i></figcaption>
	</figure>
</div>

<div style="display:flex">
	<figure style="width:50%; text-align:center">
	  <img src="/Images/equal-graph(2).png" >
	  <figcaption><i>G<sub>3</sub></i></figcaption>
	</figure>

	<figure style="width:50%; text-align:center">
	  <img src="/Images/equal-graph(3).png" >
	  <figcaption><i>G<sub>4</sub></i></figcaption>
	</figure>
</div>

---
#### Isomorphism
Informally, if two graphs are *isomorphic*, they are equal except for their vertices needing to be "relabeled". 

The two graphs shown below, $G_5$ and $G_6$, are isomorphic, though $G_5$ $\ne$ $G_6$. This relationship can be written as $G_5 \cong G_6$. 

<div style="display:flex">
	<figure style="width:50%; text-align:center">
	  <img src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/notes/Images/equal-graph.png?raw=true" >
	  <figcaption><i>G<sub>5</sub></i></figcaption>
	</figure>

	<figure style="width:50%; text-align:center">
	  <img src="/Images/isomorphic-graph(1).png" >
	  <figcaption><i>G<sub>6</sub></i></figcaption>
	</figure>
</div>

Taking the vertices of $G_5$ and labeling 
$$A \rightarrow E$$
$$B \rightarrow D$$
$$C \rightarrow C$$
$$D \rightarrow B$$
$$E \rightarrow A$$
would give us $G_6$. In fact, this is a bijective function $f : V_5 \rightarrow V_6$. 

Also, $f$ preserves edges. This means, given two graphs, $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$, $\{u, v\}$ is an edge of $G_1$ exactly when $\{f(u), f(v)\}$ is an edge of $G_2$. Basically, if you simply relabel the vertices, the edges remain "in place".