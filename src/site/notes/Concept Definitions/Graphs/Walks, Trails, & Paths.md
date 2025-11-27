---
{"dg-publish":true,"permalink":"/concept-definitions/graphs/walks-trails-and-paths/"}
---

#### Walks
For any graph $G$, a *walk* of length $n$ is a sequence $[v_0, e_1, v_1, e_2, ..., v_{n-1}, e_n, v_n]$  of vertices alternating with edges, starting and ending with a vertex, where each element is incident to the next.

* A walk is considered *closed* when $v_0 = v_n$.
* A walk is considered *open* when $v_0 \ne v_n$.

* A closed walk in which no edge is repeated (but vertices might be) is called a *circuit*.
* An open walk in which no edge is repeated (but vertices might be) is called a *trail*.
#### Trails
A trail is an open walk in which no edge is repeated.

#### Paths
A walk in which no vertices are repeated, except possibly starting and ending at the same vertex, is called a *path*. Since no vertices are repeated, no edges are repeated. Like walks, paths may be closed ($v_0 = v_n$) or open ($v_0 \ne v_n$). A closed path is called a *cycle*.