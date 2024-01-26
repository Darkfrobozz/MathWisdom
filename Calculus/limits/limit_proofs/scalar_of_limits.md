Let's consider the proposition $P_{1}$:
$$
\lim_{ n \to \infty } a_{n} = a \implies \lim_{ n \to \infty }  ka_{n} = k \cdot a
$$
To prove this, we want to start with [[discrete_limits]], defining $\varepsilon > 0$:
$$
|a_{n} - a| < \frac{\varepsilon}{k}, n > M \implies k|a_{n} - a| < \frac{k\epsilon}{k} \implies |ka_{n} - ka| < \varepsilon \implies P_{1}
$$