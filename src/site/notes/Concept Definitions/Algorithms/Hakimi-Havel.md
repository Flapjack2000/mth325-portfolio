---
{"dg-publish":true,"permalink":"/concept-definitions/algorithms/hakimi-havel/"}
---

The Hakimi-Havel algorithm checks if there exists a simple graph that corresponds to a given degree sequence.

The approach goes as follows:
1. Sort the degree sequence in non-increasing order.
2. Delete the first element, $d$, and subtract $1$ from the next $d$ elements.
3. Repeat steps $1$ and $2$ until one of the following stopping conditions are met:
	1. All of the remaining elements are equal to $0$. (A simple graph exists.)
	2. There are not enough remaining elements to subtract from in step $2$. (No simple graph exists.)
	3. One or more of the remaining elements is less than $0$. (No simple graph exists.)
#### Python: Hakimi-Havel Algorithm
```python
def hakimi_havel(degree_sequence):
	
	while True:
		# Sort elements in non-increasing order.
		degree_sequence.sort(reverse=True)
		
		# Check stopping condition 1.
		if all([d == 0 for d in degree_sequence]):
			return True
		
		# Remove and store first element.
		d = degree_sequence.pop(0)
		
		# Check stopping condition 2.
		if d > len(degree_sequence):
			return False
		
		# Decrement first d elements.
		for i in range(d):
			degree_sequence[i] -= 1
			
			# Check stopping condition 3.
			if degree_sequence[i] < 0:
				return False			
```
