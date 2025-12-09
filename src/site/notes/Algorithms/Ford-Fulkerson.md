---
{"dg-publish":true,"permalink":"/algorithms/ford-fulkerson/"}
---


>The Ford-Fulkerson method is a greedy algorithm that finds the maximum flow in a network.

The approach goes as follows:
1. Start with a flow of $0$.
2. Create a residual graph by copying the capacities in the original graph.
3. Find a path from the source to the sink where every edge along the path has a remaining residual capacity that is greater than $0$. Call this path an augmenting path.
	* If there is no augmenting path, then stop. (The current total flow is the maximum flow.)
	* If there is an augmenting path, then do the following:
		1. Calculate the minimum residual capacity along the augmenting path. 
		2. Add it to the flow of each edge in the forward direction (source to sink) along the path. 
		3. Subtract it from the flow of each edge in the reverse direction (sink to source) along the path. 
		4. Add it to the total flow.
4. Repeat step 3 until no augmenting path exists. Return the total flow.

#### Python Interpretation:
```python
def ford_fulkerson(capacity_matrix, source_node, sink_node):
    num_vertices = len(capacity_matrix)
	
    # Copy capacities into a residual matrix
    residual_matrix = [row[:] for row in capacity_matrix]
    total_flow = 0
	
    while True:
        # Track which nodes have been visited
        visited_nodes = [False] * num_vertices
        visited_nodes[source_node] = True
		
        # Keep track of the parents of each vertex
        parent_nodes = [-1] * num_vertices
		
        # For DFS
        stack = [source_node]
		
        # DFS to find augmenting path from source to sink
        path_found = False
        while stack:
            current_node = stack.pop()
            if current_node == sink_node:
                path_found = True
                break
            for next_node in range(num_vertices):
                if not visited_nodes[next_node] and residual_matrix[current_node][next_node] > 0:
                    visited_nodes[next_node] = True
                    parent_nodes[next_node] = current_node
                    stack.append(next_node)
		
        # End once max flow is found
        if not path_found:
            break
        
        # Find minimum residual capacity along the augmenting path
        min_flow = float('inf')
        node = sink_node
        while node != source_node:
            previous_node = parent_nodes[node]
            min_flow = min(min_flow, residual_matrix[previous_node][node])
            node = previous_node
			
        # Update capacites in residual matrix
        node = sink_node
        while node != source_node:
            previous_node = parent_nodes[node]
            residual_matrix[previous_node][node] -= min_flow
            residual_matrix[node][previous_node] += min_flow
            node = previous_node
		
        total_flow += min_flow
		
    return total_flow
```
