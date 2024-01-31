The question is if we have functions $f, g$ and both their derivatives are defined at $x$ then what is the derivative of their sum at that point.
$P_{1}$ is the following proposition to that question:
$$
h = f + g \implies h' = f' + g'
$$
To prove this we simply need to refer to [[derivative]]:
$$
f' = \lim_{ h \to 0 } \frac{f(x+h) - f(x)}{h} \land g' = \lim_{ h \to 0 } \frac{g(x+h) - g(x)}{h} \land h' = \lim_{ h \to 0 } \frac{f(x+h) + g(x+ h) - f(x) - g(x)}{h}
$$
Now that we have converted it to a problem of limits we can simply refer to [[sum_of_limits]], netting us:
$$
f' + g' = \lim_{ h \to 0 } \frac{f(x+h) - f(x)}{h}  + \frac{g(x+h) - g(x)}{h} = h'
$$
Proving $P_{1}$

