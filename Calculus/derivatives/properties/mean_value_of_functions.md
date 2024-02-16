We want to prove that given two functions that have [[derivative]]s on $(a,b)$, the following is true:
$$
\frac{f'(c)}{g'(c)} = \frac{f(b) - f(a)}{g(b) - g(a)}
$$
To do this we can simply first recognize by [[sum_of_derivatives]] and [[scalar_of_derivatives]] that:
$$
f(x)(g(b) - g(a)) - g(x)(f(b) - f(a))
$$
The derivative of this is then:
$$
f'(x)(g(b) - g(a)) - g'(x)(f(b) - f(a))
$$
Then according to [[mean_value_thereom]] for some point $c$, this derivative is:
$$
\frac{f(a)(g(b) - g(a)) - g(a)(f(b) - f(a)) - f(b)(g(b) - g(a)) + g(b)(f(b) - f(a))}{b - a} = \frac{0}{b - a} = 0
$$
Which gives us that :
$$
f'(c)(g(b) - g(a)) = g'(c)(f(b) - f(a)) \implies \frac{f'(c)}{g'(c)} = \frac{f(b) - f(a)}{g(b) - g(a)}
$$
$\square$