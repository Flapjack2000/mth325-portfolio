---
{"dg-publish":true,"permalink":"/algorithms/floyd-roy-warshall/"}
---


>The Floyd-Roy-Warshall algorithm (FRW) finds the lengths of the shortest paths between all pairs of vertices in a directed weighted graph.
>
>Time Complexity: $O(n^3)$

The approach goes as follows:
1. Begin with an adjacency matrix containing the weights of the edges of a graph.
2. For each vertex $i$:
	* For each vertex $k$:
		* For each vertex $j$:
			* Update the path from $k$ to $j$ if the path from $k$ to $j$ through $i$ is shorter than the current distance from $k$ to $j$.

#### Python Interpretation
```python
def floyd_roy_warshall(adj_matrix:list[list[int|float]]):
    infinity = float('inf')
    num_vertices = len(adj_matrix)
	
    # Copy adjacency matrix for initial distances
    distances = [row[:] for row in adj_matrix]
	
    for i in range(num_vertices):
        for j in range(num_vertices):
            for k in range(num_vertices):
                # Check if a shorter path is found
                if distances[k][i] != infinity and distances[i][j] != infinity:
	                path = min(distances[k][j], distances[k][i] + distances[i][j])
                    distances[k][j] = path
    return distances
```