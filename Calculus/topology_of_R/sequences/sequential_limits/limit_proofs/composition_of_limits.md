# Theory
When discussing [[discrete_limits]], it is often important, to question what happens when we work through [[compositions]].
We would want to prove $P_{1}$ that given that the input of the inner function matches that of the outer function:
$$
\lim_{ n \to \infty } a_{n} = a \land f(a) = b \land g(n) = a_{n} \implies \lim_{ n \to \infty } f \circ g (n) = b
$$
However, even though $g(n)$ approaches $a$, there is nothing in this definition that says that as the input to $f$ gets closer to $a$ the output gets closer to $b$.

# Counter Example
Below is a counter example using the set up from theory.
$$
a = 0 \land b = 5
$$
$$
f(x) = \begin{cases}
5  \impliedby x = 0 \\
1 \impliedby x \neq 0
\end{cases}
$$
Obviously, no matter how close we get to $0$, the output of $f$ will always be 4 units away from its desired limit.
Consequently, there can be no general proof for $P_{1}$.