---
{"dg-publish":true,"permalink":"/algorithms/prim-s-minimum-spanning-tree/"}
---


>Like Kruskal's algorithm, Prim's algorithm finds a minimum spanning tree (MST) of a given weighted, connected, undirected graph. Prim's algorithm is also a greedy algorithm.
>
>Time Complexity: $O(n^2)$

The approach goes as follows:
1. Choose an arbitrary current vertex. Set it's edge weight to $0$, and set all others to $\infty$.
2. Look at the current vertex's unvisited neighbors. For each unvisited neighbor, update the neighbor's edge weight if it is smaller than the currently stored weight.
3. Mark the current vertex as part of the MST.
4. Select the unvisited vertex with the smallest stored weight to be the new current vertex. Add the edge that gave it that weight to the MST.
5. Repeat steps 2 through 4 until one of the following stopping conditions is met:
	1. The MST contains all of the vertices in the graph. (The MST is complete.)
	2. The smallest weight of the remaining unvisited vertices is $\infty$. (The graph is not connected, so no MST is possible.)

#### Python Interpretation:
```python
class Edge:
    def __init__(self, v1, v2, weight):
        self.v1 = v1
        self.v2 = v2
        self.weight = weight    

def prim(graph: list[list[int]], n):
    min_weight = [float('inf')] * n
    parents = [-1] * n
    
    min_weight[0] = 0
    
    mst = []
    mst_vertices = set()
    
    for _ in range(n):
        smallest = float('inf')
        curr_vertex = -1
        
        for v in range(n):
            if v not in mst_vertices and min_weight[v] < smallest:
                smallest = min_weight[v]
                curr_vertex = v
        
        if curr_vertex == -1:
            break
        
        mst_vertices.add(curr_vertex)
        
        if parents[curr_vertex] != -1:
            edge = Edge(
	            parents[curr_vertex], 
	            curr_vertex, 
	            min_weight[curr_vertex]
            )
            mst.append(edge)
        
        for neighbor in range(n):
            if graph[curr_vertex][neighbor] > 0:
	            if neighbor not in mst_vertices:
	                if graph[curr_vertex][neighbor] < min_weight[neighbor]:
	                    min_weight[neighbor] = graph[curr_vertex][neighbor]
	                    parents[neighbor] = curr_vertex
    return mst
```