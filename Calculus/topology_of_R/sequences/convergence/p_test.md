The fundamental proposition $P_{1}$ is that for $p > 1$ the following converges:
$$
\sum_{n=1}^\infty \frac{1}{n^p} = 1+\frac{1}{2^p} + \frac{1}{3^p} + \dots 
$$
## Divergence of less or equal to zero intervals
It is very easy to prove that this is true for $p =0$ as that means we are just adding ones which means
that we can for every $M$ pick an $N > M$ such that the sum is bigger. This then diverges.

$p < 0$ this implies that we multiply each element with $n^{|p|}$, which does not converge since each element is greater than that for $p = 0$.
## Divergence of less than one
Now $p = 1$ is just the harmonic which diverges by [[divergence_of_first_harmonic]].

Anything less than $p=1$ will by comparison also diverge.

## Convergence of more than one
$$
\sum_{n=1}^\infty \frac{1}{n^p} = 1+\frac{1}{2^p} + \frac{1}{3^p} + \dots 
$$
To solve this we can use the [[cauchy_condensation]] :
$$
\sum_{n=0}^\infty 2^n \frac{1}{(2^n)^p} = \sum_{n=0}^\infty \frac{1}{2^{(1-p)n}} = \frac{\left( 1 - \left( \frac{1}{2} \right)^{(1-p)n} \right)}{1-(\frac{1}{2})^p}
$$
The sequence
$$
\frac{1}{2}^{(p-1)n}
$$
Only converges if the exponent is positive.
Moreover $p= 1$ is not a geometric sequence so that formula does not apply but we can see that it diverges since each element will be 1.