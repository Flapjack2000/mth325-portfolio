---
{"dg-publish":true,"permalink":"/algorithms/djikstra-s/"}
---




#### Python Interpretation
```python
import numpy as np

def dijkstra(graph, source):
	n = len(graph)
	distances = [float('inf') for _ in range(n)]
	distances[source] = 0
	
	for _ in range(n):
		curr_node = None
		curr_distance = float('inf')
		
		for node in range(n):
			if node not in visited and distances[node] < curr_distance:
				curr_node = node
				curr_distance = distances[node]
		
		if curr_node is None:
			break
		
		visited.append(curr_node)
		
		for neighbor in range(n):
			if graph[curr_node][neighbor] > 0:
				distance = curr_distance + graph[curr_node][neighbor]
				
				if distance < distances[neighbor]:
					distances[neighbor] = distance
	return distances
```