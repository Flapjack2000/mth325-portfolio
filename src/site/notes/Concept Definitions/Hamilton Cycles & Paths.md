---
{"dg-publish":true,"permalink":"/concept-definitions/hamilton-cycles-and-paths/"}
---


#### Hamilton Paths
A Hamilton path is a path in a connected graph that visits each vertex exactly once.
#### Hamilton Cycles
A Hamilton cycle is a Hamilton path that ends where it started. All Hamilton cycles are Hamilton paths. It's another squares and rectangles situation.

The graph below has a Hamilton cycle: $0 \to 1 \to 2 \to 3 \to 4 \to 5 \to 0$. 
Another example is this: $2 \to 3 \to 1 \to 0 \to 5 \to 4 \to 2$.


<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/hamilton.png?raw=true" >
	  <figcaption></figcaption>
	</figure>
</div>


#### The Icosian Game
The Icosian Game is a mathematical puzzle by William Rowan Hamilton. The goal is to find a path on a dodecahedron, such that the path travels along the edges of the dodecahedron, visits each of the 20 vertices exactly once, and returns to the starting vertex. This kicked off the mathematical interest in finding Hamilton cycles/paths.