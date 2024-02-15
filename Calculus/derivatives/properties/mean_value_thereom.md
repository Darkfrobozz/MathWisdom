The components we have is an interval $[a,b]$ and a function $f$ that is differentiable over this interval.
Now we can obviously produce a line with a slope $m$ such that:
$$
\frac{f(b) - f(a)}{b - a} = m, b \neq a
$$
Now what we want to prove is that the derivative at some point $c \in (a,b)$ is parallel to that line.

The proof for this is elementary once we understand that:
$$
(f(x) - mx)' = f'(x) - m
$$
By [[sum_of_derivatives]] this is then defined over the same interval and what's more, we know that from that $m$ represents the line going through $(a, f(a))$ and $(b, f(b))$ :
$$
ma = f(a) \land mb = f(b) \implies f(a) - ma = 0 \land f(b) - mb = 0
$$
Consequently, we can use [[internal_horizontal_parallel_thereom]] to conclude that:
$$
\exists c \in (a,b) : f'(c) - m = 0 \implies f'(c) = m
$$
Which is what we wanted to prove! $\square$