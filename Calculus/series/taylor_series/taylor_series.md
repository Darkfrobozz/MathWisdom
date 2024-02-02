A taylor series is a method for making an infinite [[polynomial_approximation]] of some function $f$.

It is based on that polynomials always have [[derivative]] and the [[derivative]] of a polynomial is always a polynomial :
These two facts together means that we can use derivatives to find a value for every constant in our [[polynomial_approximation]] by continuously taking derivatives.
Ultimately, by taking derivatives we can make an unknown constant separate from the variable part of the [[polynomial_approximation]] and, then, we can set that part to 0. Consequently, we are only left with the target constant.

However, this depends on that the function that we are trying to approximate is also infinitely derivable. Moreover, we can in fact not prove that the [[discrete_limits]] of this [[polynomial_approximation]] is in general the [[function]] we are trying to differentiate.

In general, we can then define a formula to find the constants of a taylor series:
$$
P_{\infty}(x) = f(a) + \frac{f'(a)}{1!}(x-a) + \dots + \frac{f^n(a)}{n!}(x-a)^n + \dots
$$