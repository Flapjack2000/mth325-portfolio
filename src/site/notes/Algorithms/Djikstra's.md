---
{"dg-publish":true,"permalink":"/algorithms/djikstra-s/"}
---

Dijkstra's algorithm finds the shortest distances from a source node to the other nodes in the graph.

The approach goes as follows:
1. Initialize the distance from the source vertex to itself as $0$. All other distances should be set to $\infty$.
2. Set the source vertex as the current vertex.
3. Look at all of the current vertex's unvisited adjacent vertices and calculate their distances from the source vertex through the current vertex. Update their respective distances if the new distance is less than the old distance.
4. Mark the current vertex as visited.
5. Look at the new distances and select the unvisited vertex with the smallest distance to be the next current vertex.
6. Repeat steps $3$ through $5$ until one of the following stopping conditions are met:
	1. Every vertex has been visited. (Shortest distances have been found successfully.)
	2. The smallest distance of the remaining unvisited vertices is $\infty$. (There is no path from the source vertex to any of the remaining unvisited vertices.)

#### Python Interpretation
```python
def dijkstra(graph: list[list[int]], source: int):
    # Count number of nodes in the graph
    n = len(graph)
    
    # Initialize all distances to infinity, source is 0
    distances = [float('inf') for _ in range(n)]
    distances[source] = 0
    
    # Keep track of which nodes have been visited
    visited = []
    
    for _ in range(n):
        # Find the unvisited node with smallest distance
        curr_node = None
        curr_distance = float('inf')
        
        for node in range(n):
            if node not in visited and distances[node] < curr_distance:
                curr_node = node
                curr_distance = distances[node]
        
        # If no reachable unvisited nodes remain, stop early
        if curr_node is None:
            break
        
        # Mark current node as visited
        visited.append(curr_node)
        
        # Update distances to all neighbors of current node
        for neighbor in range(n):
            # Check if there's an edge to this neighbor
            if graph[curr_node][neighbor] > 0:
                # Calculate distance through current node
                distance = curr_distance + graph[curr_node][neighbor]
                
                # Update if a shorter path is found
                if distance < distances[neighbor]:
                    distances[neighbor] = distance
    return distances
```