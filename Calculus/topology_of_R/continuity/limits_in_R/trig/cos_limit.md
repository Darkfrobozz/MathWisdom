We are going to use the [[sin_limit]] to prove a special limit:
$$
\lim_{ x \to 0 } \frac{\cos x - 1}{x}
$$
We will do this by manipulating the expression into something akin to the [[sin_limit]]:
$$
\lim_{ x \to 0 } \frac{(\cos x-1)(\cos x + 1)}{x(\cos x + 1)} = \lim_{ x \to 0 } \frac{\cos^2x - 1}{x(\cos x + 1)} = \lim_{ x \to 0 } \frac{-\sin^2x}{x(\cos x + 1)}
$$
Now we got sine in the top part, thus, we can continue to change this expression with [[product_of_limits]] and use the [[sin_limit]]:
$$
- \lim_{ x \to 0 } \frac{\sin x}{\cos x + 1} \lim_{ x \to 0 } \frac{\sin x}{x}
= - \lim_{ x \to 0 } \frac{\sin x}{\cos x + 1} \cdot 1
$$
Finally we can wrap it up by observing that the remaining limit goes to $0$ :
$$
- 0 \cdot 1 = 0
$$
Which gives use that the limit in the end is $0$