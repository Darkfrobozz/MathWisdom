Let's consider the following proposition $P_{1}$ about [[discrete_limits]]:
$$
\lim_{ n \to \infty } a_{n} = a \land \lim_{ n \to \infty } b_{n} = b \implies \lim_{ n \to \infty } a_{n} b_{n} = a \cdot b
$$

To prove this we will use an intermediate point $ab_{n}$ and apply the [[triangle_inequality]]:
$$
|ab - a_{n}b_{n}| \leq |ab - ab_{n}| + |ab_{n} - a_{n}b_{n}| = |a| |b - b_{n}| + |b_{n}| |a - a_{n}|
$$
Now we want to prove that $\forall \varepsilon > 0 : \exists M \in  N: n > M \implies |ab - a_{n}b_{n}| < \varepsilon$
So set $\varepsilon$ and then pick:
$$
\exists M_{1}: |b - b_{n}| < \frac{\varepsilon}{2|a|} \land \exists M_{2} : |b_{n}| \leq |2b| \land \exists M_{3} : |a-a_{n}| \leq \frac{\varepsilon}{4|b|}
$$
Now we simply pick $M = max(M_{1}, M_{2}, M_{3})$, which implies that all those conditions are true, putting it together:
$$
n > M \implies |ab - a_{n}b_{n}| \leq |a| |b - b_{n}| + |b_{n}| |a - a_{n}| \leq |a| \frac{\varepsilon}{2|a|} + \frac{2|b|\varepsilon}{4|b|} \leq \varepsilon \implies P_{1}
$$