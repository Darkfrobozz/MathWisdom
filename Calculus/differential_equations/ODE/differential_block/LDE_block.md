Let's consider the following:
$$
y' + p(x)y = q(x)
$$
This is an extension of a [[separable_block]], in fact, we can solve it by putting $q(x) = 0$ and, then, solve it as usual, we get: $y' = -p(x)y$
Given the solution on the form:
$$
y = Ke^{-u(x)} \implies y = Ke^{-u(x)}
$$
We can replace $K$ with a function $k(x)$
$$
y = k(x)e^{-u(x)}
$$
$$
y' + p(x)y = q(x) \implies (k(x)e^{-u(x)})' + p(x)k(x)e^{-u(x)} = q(x)
$$

$$
k(x)'e^{-u(x)} + k(x)p(x)e^{-u(x)} + p(x)k(x)e^{-u(x)} = q(x)
$$
$$
k'(x)e^{-u(x)} = q(x)
$$
So we have proven that so long as this derivative is 0, a constant, we will have an answer.
$$
k'(x) = \frac{q(x)}{e^{-u(x)}}
$$
So we can found the most [[simple_block]] to find $k(x)$ and getting the solution.