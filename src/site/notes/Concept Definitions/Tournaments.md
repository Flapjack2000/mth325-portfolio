---
{"dg-publish":true,"permalink":"/concept-definitions/tournaments/"}
---


#### Tournaments
A tournament is a directed graph, $T = (V, E)$, so that for every distinct pair of vertices $u \ne v$, either $(u, v) \in E$ or $(v, u) \in E$, but not both.

$(u, v) \in E$ can be written as $u \to v$.

Oftentimes, tournament graphs are used for ranking players or teams in tournaments, hence the name.
#### Rankings
A *ranking* is an ordering $v_1, v_2, ..., v_n$ of the vertices of a tournament for which the number of vertices is $n$.

A *valid ranking* is ranking of a tournament for which ${v_1 \to v_2}, {v_2 \to v_3}, ..., {v_n-2 \to v_n-1}, {v_n-1 \to v_n}$.

There may be multiple valid rankings for a given tournament. It is also possible for a tournament to not have a valid ranking.

A valid ranking for $T$, shown below, is $A, D, B, E, C$. Two more valid rankings are $A, C, D, B, E$ and $A, E, D, B, C$.

Note that because $deg^-(A) = 0$, no other vertex can come before $A$ in any valid ranking. If there were another vertex $F$, such that $v \to F$ for any vertex $v \in T$, then 
<div style="display:flex; justify-content:center;">
	<figure style="width:50%; text-align:center">
	<img style="border-radius:5%;" src="https://github.com/Flapjack2000/mth325-portfolio/blob/main/src/site/Images/tournament.png?raw=true" >
		  <figcaption>
			  <i>A tournament, T, with 5 vertices</i>
		  </figcaption>
	</figure>
</div>

