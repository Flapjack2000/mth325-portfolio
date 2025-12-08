---
{"dg-publish":true,"permalink":"/proofs/dr-wells-list-of-conjectures/"}
---

1. In a graph $G$, if there are at least 2 distinct paths from a vertex $u$ to another vertex $v$, then $G$ contains a cycle. [[Proofs/by Direct Proof/Two Distinct Paths Between Two Vertices Imply a Cycle\|Jump to Proof]]
    
2. In a connected graph $G$, if an edge $(u,v)$ is the only path from $u$ to $v$, then $(u,v)$ is a cut edge.
    
3. If $T$ is a tree, then every edge of $T$ is a cut edge. [[Proofs/by Direct Proof/All Tree Edges Are Cut Edges\|Jump to Proof]]
    
4. If $G$ is a connected graph and $\Delta(G) = \delta(G) = 2$ (all the vertices have degree 2), then $G$ is a cycle.
    
5. For any even integer $n \geq 4$, the cycle on $n$ vertices, $C_n$, is bipartite.
    
6. For any graph $G$, if $\Delta(G) \geq 2$, then $G$ has at least 3 vertices.
    
7. For any graph $G$, $|V| \geq \Delta(G) + 1$.
    
8. For any graph $G$, if $\delta(G) \geq 2$ (all the vertices have degree at least 2), then $G$ contains a cycle.
    
9. If $T$ is a tree with $n$ vertices, then $T$ has $n - 1$ edges. [[Proofs/by Induction/Weak Induction/Trees Have n-1 Edges\|Trees Have n-1 Edges]]
    
10. In any tree $T$, for any vertices $u$ and $v$, there is exactly one path from $u$ to $v$. [[Proofs/by Contradiction/Exactly One Path Between Any Two Vertices in a Tree\|Jump to Proof]]
    
11. Every tree with 2 or more vertices has leaves.
    
12. If $F$ is a forest with $n$ vertices and $k$ connected components, then $F$ has $n - k$ edges.
    
13. Let $G$ be a graph with $n$ vertices. If $G$ is connected, then $G$ has at least $n - 1$ edges.
    
14. Let $G$ be a graph with $n$ vertices. If $G$ is connected and has $n - 1$ edges, then $G$ is a tree. [[Proofs/by Contrapositive/Connected Graphs with Minimal Edges Are Trees\|Jump to Proof]]
    
15. Let $G$ be a graph with $n$ vertices. If $G$ has no cycles and has $n - 1$ edges, then $G$ is a tree.
    
16. Let $G = (V,E)$ be a graph with $|V| = n$. If $|E| \geq n$, then $G$ has (at least one) cycle.
    
17. For every positive integer $n$, if $T$ is a tournament with $n$ vertices then there is at least one admissible ranking. That is, there is a sequence of vertices $v_1, v_2, \ldots, v_{n-1}, v_n$ so $v_i \to v_{i+1}$ for $i = 1, 2, \ldots, n - 1$.
    
18. Let $T$ be a tournament and $C$ be cycle in $T$. If $C$ is maximal, then for every vertex $v$ of $T$ that is not in $C$, either for every vertex $c$ in $C$, $v \to c$, or for every vertex $c$ in $C$, $c \to v$.
    
19. Let $T$ be a tournament. If $T$ has exactly one (unique) ranking, then $T$ has no (directed) cycles.
    
20. Let $T$ be a tournament. If $T$ has more than one ranking, then $T$ contains at least one (directed) cycle.
    
21. Let $T$ be a tournament. If $T$ contains a cycle of length $k > 3$, then $T$ contains a cycle of length 3 or a cycle of length $k - 1$.
    
22. Let $T$ be a tournament. If $T$ contains a cycle, then $T$ contains a cycle of length 3.
    
23. Let $T$ be a tournament. If $T$ has exactly one (unique) ranking, then the relation represented by $T$ is transitive.
    
24. Let $T$ be a tournament. If $T$ has more than one ranking, then the relation represented by $T$ is not transitive.
    
25. If an undirected multi-graph $G$ is connected and every vertex of $G$ has even degree, then $G$ has an Euler circuit.
    
26. If an undirected multi-graph $G$ has an Euler circuit, then $G$ is connected and every vertex of $G$ has even degree.
    
27. If an undirected multi-graph $G$ is connected and every vertex of $G$ has even degree except for two vertices, say $u$ and $v$, then $G$ has an Euler trail that starts at one of $u$ and $v$ and ends at the other, but does not have an Euler circuit.
    
28. If an undirected multi-graph $G$ has an Euler trail and not an Euler circuit, then $G$ is connected and every vertex of $G$ has even degree except for the vertices at the beginning and end of the trail.
    
29. If a directed multi-graph $D$ is weakly connected and every vertex of $D$ has in-degree equal to out-degree, then $D$ has a directed Euler circuit.
    
30. If a directed multi-graph $D$ has a directed Euler circuit, then $D$ is strongly connected and every vertex of $D$ has in-degree equal to out-degree.
    
31. If a directed multi-graph $D$ is weakly connected and every vertex of $D$ has in-degree equal to out-degree except for a vertex $u$ with $\deg^+(u) = \deg^-(u) + 1$ and a vertex $v$ with $\deg^+(v) = \deg^-(v) - 1$, then $D$ has a directed Euler trail that starts at $u$ and ends at $v$.
    
32. If a directed multi-graph $D$ has a directed Euler trail and not a directed Euler circuit, then $D$ is weakly connected and every vertex of $D$ has in-degree equal to out-degree except for the vertex $u$ at the beginning of the trail with $\deg^+(u) = \deg^-(u) + 1$ and the vertex $v$ at the end of the trail with $\deg^+(v) = \deg^-(v) - 1$.
    
33. For any directed graph $D$ with $n$ vertices, $D$ is strongly connected if and only if its transitive closure is the complete digraph on $n$ vertices.
    
34. For any directed graph $D$, $D$ is weakly connected if and only if its symmetric closure is strongly connected.