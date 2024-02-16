To introduce limits, we can think about [[sequence]], specifically the following $(a_{n})$
$$
(a_{n}) = (0.1, 0.01, 0.001, \dots)
$$
Now on inspection, it is clear that this sequence moves towards 0. The representation for this is:
$$
\lim_{ n \to \infty }{a_{n}} = 0 
$$
To formalize this whole notion, let's introduce a variable:
$$
\varepsilon\ |\ \varepsilon > 0 
$$
Now if we can pick an *M* for each $\varepsilon$ such that:
$$
n > M \implies (a_{n} - 0) < \varepsilon 
$$
Then, we have that:
$$
\lim_{ n \to \infty } {a_{n}} = 0
$$
