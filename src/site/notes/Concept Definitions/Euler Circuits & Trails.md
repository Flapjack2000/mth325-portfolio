---
{"dg-publish":true,"permalink":"/concept-definitions/euler-circuits-and-trails/"}
---

#### Euler Trails
An *Euler trail* is a trail $t$ in a graph, such that $p$ travels along every edge in the graph exactly once. 


#### Euler Circuits
An *Euler circuit* is a trail $t$ in a graph, such that $p$ starts and ends at the same vertex and travels along every edge in the graph exactly once.

Note that an Euler circuit is simply an Euler trail that starts and ends at the same vertex. It's a squares and rectangles situation.


<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/euler-trail.png?raw=true" >
	  <figcaption><i>G<sub>1</sub></i></figcaption>
	</figure>
</div>

Notice that $G_1$, shown above, does not have an Euler circuit but does have an Euler trail.
$$A \to B \to C \to D$$