To prove this consider first :
$$
\sum_{n=1}^\infty \frac{1}{n} = 1 + \frac{1}{2} + \frac{1}{3} + \dots
$$
Now obviously $\frac{1}{n}$ moves towards zero but consider if we made a smaller sequence then if that diverges this must also diverge.
Thus, we construct :
$$
\begin{align}
&1 + \frac{1}{2} + \frac{1}{4} + \frac{1}{4} + \frac{1}{8} + \frac{1}{8} + \frac{1}{8} + \frac{1}{8} + \dots\\ \\
&1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} + \frac{1}{5} + \frac{1}{6} + \frac{1}{7} + \frac{1}{8} + \dots
\end{align}
$$
Now obviously the one below must be less since each term is less than that above.
What we are doing here is simply grabbing the distance between each power of two and putting each term to be the bigger power of two so that they are as a result all smaller than their counterpart in the harmonic.
But the distance between each power of two is :
$$
2^n - 2^{n-1} = 2^{n-1}
$$
Which implies that we will have that many terms for each time we do this but this also means that:
$$
\frac{1}{2^{n}} \cdot 2^{n-1} = \frac{1}{2}
$$
so we can reduce the series to a series of halves :
$$
\frac{1}{2} + \frac{1}{2} + \frac{1}{2} + \dots
$$
Which diverges as we can pick any $M$ and pick $N = 2M$ to produce that number.
So our lower bound series diverges which means the harmonic must diverge as well.