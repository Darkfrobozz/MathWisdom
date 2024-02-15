We want to prove that for a function $f$ that is differentiable over $[a,b]$, we have that all derivatives between the two end points occur in the interval.
Note that we assume $f'(a) < f'(b)$ for the reverse, the argument remains roughly the same.
First we fix some value $c$ such that $f'(a) < c < f'(b)$ then we augment $f(x)$ with $f(x) - cx$
This is of course also differentiable by [[sum_of_derivatives]] and [[scalar_of_derivatives]].

Now we use that the [[derivative]] implies that $f(x) - cx$ has [[continuity]] over $[a,b]$ and using that with [[existence_of_extremum]] implies that there is an extremum.
This implies by [[derivative_at_internal_extremum]] that there exists a point where the derivative is zero if that maximum is not at the end points.
Consequently, we can simply use our premise :
$$
f'(a) - c < 0 < f'(b) - c
$$
This tells us that we are decreasing at $a$ and increasing at $b$, which implies that if we should be able to find a value less than $a$ to the right of $a$ and a value less than $b$ to the left.
In either case, the minimum cannot be at the endpoint, which means that we have that there is an [[derivative_at_internal_extremum]].
Consequently there exists a point $k$:
$$
f'(k) - c = 0 \implies f'(k) = c
$$
This of course means that we have found our point for an arbitrary $c$ $\square$
