Discrete powers are interested in :
$$
x^n, n \in Z
$$

## Positive Integers
To prove this we will use induction with the following $P_{1}$ :
$$
(x^n) = nx^{n-1} 
$$
Observe for $n = 1$, the [[derivative]] definition gives us :
$$
(x)' = \lim_{ h \to 0 } \frac{x+h - x}{h} = 1 = 1 \cdot x^0 \tag{1}
$$
Thus, the rule holds for $n = 1$ :

Let's assume that it is true for $n = k -1$ :
$$
(x^{k-1}) = (k-1)x^{k-2}
$$
Now let's use the [[product_of_derivatives]] to prove it for $n = k$ :
$$
x^k = x^{k-1} \cdot x = (k-1)x^{k-2}x + x^{k-1} = (k-1 + 1)x^{k-1} = kx^{k-1}
$$
Thus, we find by mathematical induction that since (1) is true and any $k - 1 \implies k$ is true, all positive integers above $1$ are true. $\square$
## Negative Integers
To solve this we simply need to calculate $(\frac{1}{x})'$ :
$$
\lim_{ h \to 0 } \frac{\frac{1}{x + h} - \frac{1}{x}}{h} = \lim_{ h \to 0 } \frac{x - x - h}{h(x+h)(x)} = -\lim_{ h \to 0 } \frac{1}{(x+h)x} = -\frac{1}{x^2}
$$
Now we can apply the chain rule and negative integer can be seen as :
$$
f = x^n \land g = \frac{1}{x} \implies g \circ f(x) = \frac{1}{x^n}
$$
Now applying the [[chain_rule]] :
$$
(g \circ f(x))' = g'(f(x))f'(x) \\implies -\frac{1}{f(x)^2}nx^{n-1} = -\frac{n}{x^{2n}}\cdot x^{n - 1} = -\frac{n}{x^{n + 1}}
$$
Using this conclusion we have that :
$$
(x^n)' = nx^{n-1}
$$
is true for negative integers too. $\square$
