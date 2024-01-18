## [[discrete_limits]] Motivation
To introduce continuous limits, one approach is to use continuous mappings such as [[function]]s.

For example, let's define a function *f*
$$
f(x) = x
$$
Q: Now what is a limit to some point in terms of *f*?
$$
\lim_{ x \to 1 }f(x) =\ ?
$$
Essentially we define the limit as if and only if all sequences towards some point have the same [[discrete_limits]], then, we have a continuous limit at that point and the continuous limit equals these [[discrete_limits]].
## Example
$$
(a_{n}) = (1.1, 1.01, 1.001, 1.0001, \dots) \implies \lim_{ n \to \infty } f((a_{n})) = 1 \implies \lim_{ x \to 1 } = 1  
$$

Note that the last bit only follows if all the other [[discrete_limits]] are equivalent.
Q: We can't possibly test every sequence?

However, we can generalize all these sequences by noting what is implied by their [[discrete_limits]]:
$$
\lim_{ n \to \infty } (b_{n}) = 1 \land \varepsilon \ > 0 \implies  \exists M: n > 0 \implies | b_{n} - 1 | < \varepsilon   
$$
Now we can use the definition of the function *f* to prove that all the limits will approach 1 :
$$
f(b_{n}) = b_{n} \implies |f(b_{n}) - 1| = | b_{n} - 1 | \implies |f(b_{n}) - 1| < \varepsilon
$$
Thus, for any such sequence produced by putting $b_{n} \to 1$, we find that putting that sequence as input in this function *f* results in it approaching 1. 
Thus,
$$
\lim_{ x \to 1 } f(x) = 1
$$
## Acknowledgement
There are alternative ways to define continuous limits, for all those ways, it is important to check that they actually work in unison with the other standard ways of defining continuous limits.