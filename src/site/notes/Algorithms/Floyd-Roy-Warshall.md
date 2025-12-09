---
{"dg-publish":true,"permalink":"/algorithms/floyd-roy-warshall/"}
---


The Floyd-Roy-Warshall algorithm (FRW) finds the lengths of the shortest paths between all pairs of vertices in a graph.


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