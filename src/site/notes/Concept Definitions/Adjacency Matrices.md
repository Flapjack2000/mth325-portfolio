---
{"dg-publish":true,"permalink":"/concept-definitions/adjacency-matrices/"}
---


#### Adjacency Matrices
An adjacency matrix is a way of representing a graph by using a square matrix with a number of rows and columns equal to the number of vertices in the graph's vertex set.

They can be used for undirected and directed graphs, as well as unweighted and weighted graphs.

For undirected graphs, the matrix is symmetric because an edge connects its incident vertices both ways. For directed graphs, the matrix can be asymmetric because the edge are directional.

For the adjacency matrix $A$ of any directed graph $G$, the transpose of $A$, $A^T$, is the adjacency matrix obtained by reversing the direction of every edge in $G$.

For unweighted graphs, the entries are either $0$ or $1$ to represent the absence or presence of an edge. For weighted graphs, the entries are the edges' weights with a special value (such as $0$ or $\infty$) to denote no connection between vertices.

###### Undirected & Unweighted
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/adjmat-00.png?raw=true" >
	  <figcaption><i>G<sub>1</sub></i></figcaption>
	</figure>
</div>


$$
\begin{bmatrix}     
0 & 0 & 1 & 0 & 1 & 1 \\  
0 & 0 & 0 & 0 & 1 & 1 \\     
1 & 0 & 0 & 1 & 1 & 0 \\     
0 & 0 & 1 & 0 & 0 & 0 \\     
1 & 1 & 1 & 0 & 0 & 1 \\     
1 & 1 & 0 & 0 & 1 & 0 \\     
\end{bmatrix}
$$
 



###### Undirected & Weighted
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/adjmat-01.png?raw=true" >
	</figure>
</div>


$$
\begin{bmatrix}     
0 & 0 & 3 & 0 & 7 & 9 \\  
0 & 0 & 0 & 0 & 2 & 8 \\     
3 & 0 & 0 & 1 & 4 & 0 \\     
0 & 0 & 1 & 0 & 0 & 0 \\     
7 & 2 & 4 & 0 & 0 & 6 \\     
9 & 8 & 0 & 0 & 6 & 0 \\     
\end{bmatrix}
$$



###### Directed & Unweighted
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/adjmat-10.png?raw=true" >
	</figure>
</div>


$$
\begin{bmatrix}     
0 & 0 & 1 & 0 & 1 & 1 \\  
0 & 0 & 0 & 0 & 1 & 1 \\     
0 & 0 & 0 & 1 & 1 & 0 \\     
0 & 0 & 0 & 0 & 0 & 0 \\     
0 & 0 & 0 & 0 & 0 & 1 \\     
0 & 0 & 0 & 0 & 0 & 0 \\     
\end{bmatrix}
$$



###### Directed & Weighted
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	  <img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/adjmat-11.png?raw=true" >
	</figure>
</div>


$$
\begin{bmatrix}     
0 & 0 & 3 & 0 & 7 & 9 \\  
0 & 0 & 0 & 0 & 2 & 8 \\     
0 & 0 & 0 & 1 & 4 & 0 \\     
0 & 0 & 0 & 0 & 0 & 0 \\     
0 & 0 & 0 & 0 & 0 & 6 \\     
0 & 0 & 0 & 0 & 0 & 0 \\     
\end{bmatrix}
$$

