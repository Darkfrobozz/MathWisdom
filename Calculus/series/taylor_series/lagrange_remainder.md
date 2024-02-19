Given some [[taylor_series]], there exists some difference between it and the [[function]] it approximates.
We call this difference the lagrange remainder $R_{n}$.

We now want to prove the following proposition $P_{1}$ through mathematical induction:
$$
R_{n}(x) = \frac{f^{n+1}(s)}{(n+1)!}(x-a)^{n+1}
$$
And $s$ here is some value between $a$ and $x$.

Note that for $n = 0$, we can see that this formula is true since it is given by the [[mean_value_thereom]] ($x$ is the endpoint here) :
$$
f(x) = f(a) + f'(s)(x-a) \implies \frac{f(x) -f(a)}{x-a} = f'(s) \tag{1}
$$
Now let's assume that $P_{1}$ is true for $n = k - 1$ for all functions :
$$
R_{k-1}(x) = \frac{f^k(s)}{k!}(x-a)^k
$$
Let's now consider $R_{k}(x)$ and use the [[mean_value_of_functions]] on the functions $R_{k}(t)$ and $(t-a)^{k+1}$.
Note that since the Taylor series is centred on *a* the remainder there, $R_{k}(a)$, is necessarily zero.
$$
\frac{R_{k}(x) - R_{k}(a)}{(x-a)^{k+1} -(a-a)^{k+1}} = \frac{R_{k}(x)}{(x-a)^{k+1}} = \frac{R_{k}'(u)}{(k+1)(u-a)^k} \tag{2}
$$
Now we simply need to figure out what $R_{k}'(u)$ is:
$$
R_{k}(t) = f(t) - T_{k}(t)
$$
$$
R_{k}(t) = f(t) - f(a) - \frac{f'(a)}{1!}(t-a) - \dots - \frac{f^{k}(a)}{k!}(t-a)^k
$$
Differentiating this we find that:
$$
R_{k}'(t) = f'(t) - f'(a) - \dots -  \frac{f^k(a)}{(k-1)!}(t-a)^{k-1}
$$
This is the *k-1*th remainder of $f'(x)$.
Using the induction assumption then again we find that:
$$
R'_{k}(t) = \frac{(f')^k(s)}{k!} (u-a)^k = \frac{f^{k+1}(s)}{k!}(u-a)^k
$$
Now bringing this into $(2)$ we find that :
$$
\begin{align}

R_{k}(x) &= \frac{f^{k+1}(s)}{k!}(u-a)^k \frac{(x-a)^{k+1}}{(k+1)(u-a)^k} \\
&= \frac{f^{k+1}(s)}{(k+1)!}(x-a)^{k+1}

\end{align}
$$
Consequently, given that $P_{1}$ is true for $R_{k-1}$ we have that it is true for $R_{k}$. Thus, by mathematical induction, we have that it is true for case 0 by (1) and, thus, true for all cases. $\square$