Let's consider [[discrete_limits]], there are two parts to consider here:
$$
\lim_{ n \to \infty } a_{n} + b_{n} \equiv \lim_{ n \to \infty } a_{n} + \lim_{ n \to \infty } b_{n}
$$
Let's consider some $\varepsilon$ and let the limits be *a* and *b* respectively:
$$
\left( n > M_{1} \implies |a_{n} - a| < \frac{\varepsilon}{2} \right) \land \left( n > M_{2} \implies |b_{n} - b| < \frac{\varepsilon}{2} \right)
$$
Now let's take $M = max(M_{1}, M_{2})$.
$$
n > M \implies |a_{n} - a| + |b_{n} - b| < \varepsilon
$$
This allows us to use the triangle identity:
$$
|a_{n} + b_{n} - a - b| < |a_{n} - a| + |b_{n} - b| < \varepsilon
$$
To conclude that if the corresponding limits exist then:
$$
\lim_{ n \to \infty } a_{n} + b_{n} = a + b
$$