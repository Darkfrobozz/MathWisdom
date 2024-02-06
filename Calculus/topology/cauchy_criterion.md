## [[discrete_limits]] implies Cauchy
In [[discrete_limits]] we formalize convergence in this specific way:
$$
\lim_{ n \to \infty } x_{n} = x
$$
if and only if we can always find an $N$ for which all $n$ above that leads to arbitrarily close values of the sequence to the limit.

But another way to view this is the following:
Consider the sequence $x_{n}$ again, then, we can be absolutely sure that :
$$
n > N: |x_{n} - x| < \varepsilon \implies n,m > N : |x_{n} - x_{m}| < 2\varepsilon
$$
We can prove this by the [[triangle_inequality]] :
$$
|x_{n} - x_{m}| \leq |x_{n} - x| + |x - x_{m}| < 2\varepsilon 
$$
This relationship between elements of the sequence is the cauchy criterion and we can see that [[discrete_limits]] implies this relationship $\square$ 
But is the reverse true?

## Cauchy implies [[discrete_limits]]
Assume that :
$$
n,m > N: |x_{n} - x_{m}| < \varepsilon
$$
To prove this we first need to prove that such a sequence's tail must be bounded and to prove that we can simply put forward that the following is an upper bound:
$$
x_{N} + \varepsilon
$$
If it were not an upper bound then there exists $x_{m} > x_{N} + \varepsilon$
That would mean :
$$
x_{m} - x_{N} > \varepsilon
$$
Which is a contradiction, thus, we can conclude that it is bounded and by [[axiom_of_completeness]], we have that there exists a least upper bound.
Similarly, we can prove that there exists a greatest lower bound.

Putting these two together we have that the maximum difference between these are $2\varepsilon$ which means that the difference for arbitrary $N$ can be made as close to zero as possible.
We can call the sequence of greatest lower bound $b_{n}$ and that of least upper bounds $a_{n}$.
Now because $a_{n}$ is bound by $b_{n}$ we have that $a_{n}$ has a greatest lower bound and since the difference goes towards zero that lower bound must be the least upper bound of $b_{n}$ and in fact then this bound is an acceptable answer to the limit of our cauchy sequence. $\square$

This means that the cauchy criterion implies the existence of a [[discrete_limits]]
## Equivalence
Concluding we can combine these two parts to observe that :
Cauchy criterions are equivalent with [[discrete_limits]].