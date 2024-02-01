The chain rule is about the composition of derivatives, what is the relation between $f', g'$ and $(f \circ g)'$
There are different reasonings behind this but let's focus on the [[linear_approximation]] part of [[derivative]]s.
Specifically, we know that the derivative gives us an approximation for:
$$
f(x + h) \approx f(x) + f'(x)h \land g(x + h) \approx g(x) + g'(x)h 
$$
Let's chain these parts together:
$$
f(g(x + h)) \approx f(g(x) + g'(x)h)
$$
Notice that for small values of *h* the part g'(x)*h* approaches zero as $g'(x)$ is constant at any fixed point.
This implies that we can look at $g'(x)h$ as $h$ and $g(x)$ as $x$ from our earlier approximations:
$$
f(g(x +h)) \approx f(g(x)) + f'(g(x))g'(x)h
$$
But we also know that:
$$
f(g(x+h)) \approx (f(g(x)))'h \implies (f(g(x)))' = f'(g(x))g'(x)
$$