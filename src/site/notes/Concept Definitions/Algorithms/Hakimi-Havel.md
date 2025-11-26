---
{"dg-publish":true,"permalink":"/concept-definitions/algorithms/hakimi-havel/"}
---


The Hakimi-Havel algorithm checks if there exists a simple graph that corresponds to a given degree sequence.

The approach goes as follows:

1. Sort the degree sequence in non-increasing order.
2. Delete the first element, $d$, and subtract $1$ from the next $d$ elements.
3. Repeat step 2 until one of the following stopping conditions are met:
	1. All of the remaining elements are equal to $0$.
	2. There are not enough remaining elements to subtract from in step 2.
	3. One or more of the remaining elements is less than $0$.



```Python
while True:

```