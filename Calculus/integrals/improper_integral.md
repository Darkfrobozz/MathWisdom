Under the [[existence_of_integral]]s, we can apply the [[anti_derivative_thereom]] over a [[continuity]] interval. However, what happens when there is no [[continuity]] or the interval is not bounded.
That is where improper integrals come into play. For example, consider the the integral:
$$
\int _{0}^\infty f(x) \, dx 
$$
This is not on a bounded interval and even if there is continuity, we can not apply the [[anti_derivative_thereom]]. Therefore, we instead focus on a sequence produced by :
$$
a_{n} = \int _{0}^{g(n)} f(x) \, dx 
$$
such that $g(n) \to \infty$, now given that $f(x)$ has [[continuity]], we can apply the [[anti_derivative_thereom]] for each element: $a_{n}$ and we, thus, calculate the improper integral as:
$$
\lim_{ n \to \infty } a_{n} = \int _{0}^{\infty}f(x) \, dx 
$$