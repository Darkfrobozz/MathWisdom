Suppose $(a_{n})$ is decreasing and $a_{n} \geq 0$ for all $n \in N$

Then 
$$
\sum_{n=1}^\infty a_{n} \tag{1}
$$
converges if and only if
$$
\sum_{n=0}^\infty 2^na_{2^n} \tag{2}
$$
converges.

First let's observe the difference between $2^n$ and the previous element $2^{n-1}$ :
$$
2^n - 2^{n-1} = 2^{n-1}
$$
So we know that the number of elements in the original between 
$$
a_{2^{n-1}} \to a_{2^{n}}
$$
is exactly $2^{n-1}$
So the number of elements with a value that is greater than $a_{2n}$ is $2^{n-1}$, which is just a factor of from (2).
Consequently we know that we can create (2) by replacing each $a_{n}$ by the upper $a_{2^k}$ they fall between, each such segment of (2) must be correspondingly lower than (1) :
This means that if it diverges (1) must diverge. Consequently $(1) \implies (2)$

However, what if we use the factors provided in $(2)$ then we quickly see that what we instead can do is map the bigger of the two $a_{2^k}$ an element falls in between as a replacement.
Thus, the values will always be bigger and we have that if (1) diverge then (2) must diverge, which means that $(2) \implies (1)$.