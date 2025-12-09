---
{"dg-publish":true,"permalink":"/algorithms/kruskal-s-minimum-spanning-tree/"}
---

>Kruskal's algorithm finds a minimum spanning tree of a given weighted, connected, undirected graph. The algorithm is a greedy algorithm.
>
>Time Complexity: $O(|E| \cdot log (|V|))$

The approach goes as follows:
1. Sort all edges in the graph by weight in non-decreasing order.
2. Create an empty set to store the edges of the minimum spanning tree.
3. For each edge in the sorted list of edges, check if adding this edge to the minimum spanning tree would create a cycle (and therefore remove its status as a tree).
	1. If a cycle is formed, do not add this edge to the minimum spanning tree, and skip to the next edge.
	2. If a cycle is not formed, add the edge to the minimum spanning tree, then move to the next edge in the list.
4. Repeat step 3 until the minimum spanning tree contains $n-1$ edges, where $n$ is the number of vertices in the original graph. The minimum spanning tree is complete.

Note: If the graph is disconnected, the algorithm will create a minimum spanning forest instead.

#### Python Interpretation:
```python
class Edge:
	def __init__(self, v1, v2, weight):
		self.v1 = v1
		self.v2 = v2
		self.weight = weight

class DisjointSet:
	def __init__(self, n):
		self.parent = list(range(n))
	
	def find(self, e):
		if self.parent[x] != x:
			self.parent[x] = self.find(self.parent[x])
		return self.parent[x]
	
	def union(self, x, y):
		parent_x, parent_y = self.find(x), self.find(y)
		if parent_x == parent_y:
			return False
		self.parent[parent_y] = parent_x
		return True

def kruskal(edges):
	vertices = set()
	for edge in edges:
		vertices.update([e.v1, e.v2])
	n = max(vertices) + 1
	
	edges.sort(key=lambda e: e.weight)
	
	ds = DisjointSet(n)
	mst = []
	
	for edge in edges:
		if ds.union(e.v1, e.v2):
			mst.append(e)
	return mst
```