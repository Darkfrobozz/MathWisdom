The lagrange error bound proves to be a vital piece of [[taylor_series]] as we cannot prove that in general this [[taylor_series]] is a perfect approximation of the target [[function]].

Thus, we need to prove that for each target [[function]]
$$
\lim_{ n \to \infty } T_{n}(x) = f(x)
$$
Then, we can use the [[lagrange_remainder]] of a taylor series :
$$
R_{n}(x) = f(x) - T_{n}(x)
$$
Consequently, if :
$$
\lim_{ n \to \infty } R_{n} = 0 \implies \lim_{ n \to \infty } T_{n}(x) = f(x)
$$
So if, 
$$
\lim_{ n \to \infty } \frac{f^{n+1}(s)}{(n+1)!}(x-a)^{n+1} = 0
$$
Then, we have that it is a perfect approximation.