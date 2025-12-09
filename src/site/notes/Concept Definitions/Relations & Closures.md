---
{"dg-publish":true,"permalink":"/concept-definitions/relations-and-closures/"}
---



#### Reflexive and Irreflexive Relations
A relation on a set is *reflexive* if **every** element is related to itself.
Example: 
* "is equal to"
* Every number is equal to itself.

A relation on a set is *irreflexive* if **no** element is related to itself.
Example: 
* "is a parent of"
* A person cannot be a parent of themselves.

It's important to note that a relation can be neither reflexive nor irreflexive. This happens when some elements are related to themselves and some are not.

#### Symmetric and Antisymmetric Relations
A relation on a set is *symmetric* if whenever one element is related to another, the reverse is also true.
Example:
* "is a sibling of"
* Zach is a sibling of Nick, and Nick is a sibling of Zach.

A relation on a set is *antisymmetric* if whenever two elements are related in both directions, they must be the same element.
Example:
* "is less than or equal to"
* If $a \leq b$ and $b \leq a$, then $a = b$.

Note that a relation can be both symmetric and antisymmetric or neither symmetric nor antisymmetric.

#### Transitive and Antitransitive Relations
A relation on a set is *transitive* if whenever an element is related to a second element and the second element is related to a third element, then the first element is also related to the third element.
Example:
* "is greater than"
* If $a > b$ and $b > c$, then $a > c$.

A relation on a set is *antitransitive* if whenever an element is related to a second element and the second element is related to a third element, then the first element cannot be related to the third element.
Example:
* "is the mother of"
* If Jeanette is the mother of Joanna, and Joanna is the mother of Zach, then Jeanette is not the mother of Zach.
#### Equivalence Relations
An *equivalence relation* is a relation that is reflexive, symmetric, and transitive.
#### Partial Orders
A *weak partial order* is a relation that is reflexive, antisymmetric, and transitive.
A *strong partial order* is a relation that is irreflexive, antisymmetric, and transitive.
A weak partial order can simply be called a partial order.
#### Closures of Relations
A closure of a relation is the smallest added set of ordered pairs required to fulfill a specific property, such as transitivity or symmetry.

For example, to form symmetric closure on a directed graph $G=(V, E)$, one would add the reverse of every existing edge to the graph's edge set. That is, the new set of edges for the symmetric closure of $G$ is $E \cup \{(v, u)\ |\ (u, v) \in E\}$.

Perhaps the vertices of the directed graph denote users on LinkedIn and a directed edge from a vertex $u$ to another vertex $v$ indicates that $u$ is a connection of $v$$. On LinkedIn, connections are two-way, so the relation is symmetric.