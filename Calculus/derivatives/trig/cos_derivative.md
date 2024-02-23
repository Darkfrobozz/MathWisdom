We could start from defintions but we can also build upon [[sin_derivative]] by using a trig identity and [[chain_rule]]:
$$
\cos x = \sqrt{ 1 -  \sin^2 x }
$$
Thus, we can now take the derivative:
$$
(\sqrt{ 1 - \sin^2 x })' = \frac{1}{2\sqrt{ 1 - \sin^2x }} \cdot -2\sin x \cdot \cos x = -2 \sin x
$$
Notice that this only works for positive values of $\cos x$
To resolve that issue we need to notice that:
$$
\cos x =
\begin{cases}
\sqrt{ 1 - \sin^2x }, \cos x \geq 0 \\
-\sqrt{ 1 - \sin^2x }, \cos x < 0
\end{cases}
$$
How does this affect the derivative?
Well [[scalar_of_derivatives]] tells us that the negative part is simply retained:
$$
(\pm \sqrt{ 1 - \sin^2x })
= \pm\frac{1}{2\sqrt{ 1 - \sin^2x }} \cdot -2\sin x \cdot \cos x
$$
Then for the cases we have that the negative scale cancels out the negative part for $\cos x$ so that only $-\sin x$ is left.
Thus, we have addressed both cases and see that it holds in general.