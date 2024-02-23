We can generalize the idea of the [[chain_rule]] to any function $f(x)$, the chain rule informs us that:
$$
\frac{d(f(g(x)))}{dx}  = f'(g(x))g'(x)
$$
So assuming that it is true for our function we have that we can make progress in a derivative even if we don't know what the derivative of $g$ is.
That is implicit differentiate. We often even drop the fact that these are functions and write
$$
g(x) = y \land f(g(x)) = f(y) \implies (f(y))' = f'(y) \cdot y'
$$
This can be incredibly useful when we want to find the derivative of $g(x)$ indirectly.