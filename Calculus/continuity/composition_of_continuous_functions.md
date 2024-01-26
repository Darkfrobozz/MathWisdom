When we discussed [[discrete_limits]], we found that [[composition_of_limits]] did not result in desirable behaviour.
However, does the [[compositions]] of continuous [[function]]s result in a continuous function?

To start this proof let's make the proposition $P_{1}$ clear:

$$
f, g \ \text{are continuous and composable} \implies h = f \circ g \land h \ \text{is continuous}
$$
To prove this pick a point of $g$ [[domain]] $a$, then we have that by our definition of [[continous_limits]]:
$$
\lim_{ x \to a } g(x) = g(a) \implies \forall x_{n} \to a : \lim_{ n \to \infty } g(x_{n}) = g(a)
$$
Now we simply need to prove $P_{2}$; that given any arbitrary such sequence $g(x_{n})$ that $f(g(x_{n})) \to f(g(a))$.
But here we will use the fact that $f$ has [[continuity]], which means that any sequence towards an input will move towards the output of that input.
Consequently, we have that for an arbitrary sequence that $P_{2}$ holds, this means by [[continous_limits]] that the limit at point $a$ $h$ is continuous. 
However, by the properties of [[compositions]] that the [[domain]] of $h$ is that of $g$ and that $a$ was an arbitrary point of the [[domain]] of $g$.
We have that this holds for every point of the $h$ and, consequently, $P_{1}$ is proven.