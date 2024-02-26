Given some [[serie]]s let's deconstruct it into a positive and negative version.
That is if $a_{i} < 0$ then $a_{i} \in (a_{i_{1}})$ and $a_{i} \geq 0$ then $a_{i} \in a_{i_{2}}$: 
$$
\sum a_{i} = \sum a_{i_{1}} - \sum a_{i_{2}}
$$
Now these two subsequence are obviously bounded by :
$$
\sum |a_{i}|
$$
Thus, if the absolute series converges then the two subsequences converge by [[bounded_monotone]] and since they relate in a specific way to the whole series, we have that it must converge.
So, converge of absolute series implies convergence of series.