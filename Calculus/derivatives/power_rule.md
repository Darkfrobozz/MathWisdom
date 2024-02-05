## the Square Derivative lemma
To prove that the power rule is always true, we will prove $P_{1}$ :
$$
(\sqrt{ x })' = \frac{1}{2\sqrt{ x }}
$$
First let's use the [[derivative]] definition and multiply by the rational conjugate :
$$
(\sqrt{ x })' = \lim_{ h \to 0 } \frac{\sqrt{ x + h } - \sqrt{ x }}{h} = \lim_{ h \to 0 }  \frac{(\sqrt{ x + h } - \sqrt{ x })(\sqrt{ x +h } + \sqrt{ x })}{h(\sqrt{ x+h } +\sqrt{ x })}
$$
Now we can simplify this :
$$
\lim_{ h \to 0 } \frac{x+h - x}{h(\sqrt{ x + h } + \sqrt{ x })} = \lim_{ h \to 0 } \frac{1}{\sqrt{ x+h } + \sqrt{ x }} = \frac{1}{2\sqrt{ x }}
$$
This proves $P_{1}$ $\square$
## All Multiplications with $\frac{1}{2}$ lemma
Let's think of the set of rational numbers such that :
$$
n \in N, k \in N \implies x^{\frac{n}{2^k}} 
$$
We will ignore negative numbers for the sake of this proof, now we will establish $P_{2}$ and prove it through induction for each $k$:
$$
\left( x^{\frac{n}{2^k}} \right)' = \frac{n}{2^k}x^{\frac{n}{2^k} - 1}
$$
Starting with $k = 0$, we have that :
$$
(x^n)' = nx^{n-1}
$$
Which is true by [[discrete_power_rule]], now assume that it is true for $k = l - 1$ :
$$
x^{\frac{n}{2^{l-1}}} = \frac{n}{2^{l-1}}x^{\frac{n}{2^{l-1}} - 1}
$$
Now is it true for $k = l$:
$$
(x^\frac{n}{2^{l}})' = (\sqrt{ x^{\frac{n}{2^{l - 1}}} })
$$
We can, thus, use the power rule :
$$
\frac{1}{2\sqrt{ x^\frac{n}{2^{l-1}} }} \frac{n}{2^{l-1}}x^{\frac{n}{2^{l-1}} - 1} = \frac{n}{2^l} x^{\frac{n}{2^{l-1}} - 1 - \frac{n}{2^l}} 
$$
Simplifying this further:
$$
\frac{n}{2^l} x^{\frac{n}{2^{l}} - 1} 
$$
This is of course what we were looking for and, thus, by mathematical induction it is true for all positive integers that $l$ can be. $\square$
## Tying the Lemmas Together
Let's pick some number on the number line $x$ :
This should then satisfy $n - 1 \leq x \leq n$ for some $n$ :
Pick $c_{1} = n - \frac{1}{2}$
Then $x$ is either to the right or left of $c_{1}$, choose $c_{2}$ such that it is in the same direction :
For example :
$c_{2} = n - \frac{1}{4} + \frac{1}{2}$
Now we continue this process, as we divide the segment into smaller and smaller segments, we know that $x$ as it is in the segment that we are dividing, is in one of the smaller segment. 
However, the size of the segments is going towards zero and as $c_{n}$ is either the left or right part of the segment that $x$ is in, we know that:
$$
\lim_{ n \to \infty } |c_{n} - x| = 0
$$
In other words, if we pick any number $t$ to have as our exponent :
$$
\lim_{ n \to \infty } x^{c_{n}} = x^t
$$
Moreover:
$$
c_{n} = n - \frac{1}{2} \pm \frac{1}{4} \pm \frac{1}{8} \pm \frac{1}{16} \pm \dots \frac{1}{2^n}
$$
But multiply all denominators such that :
$$
\frac{2^nn}{2^n} - \frac{2^{n-1}}{2^n} \pm \frac{2^{n-2}}{2^n} \pm \dots \frac{1}{2^n}
$$
The numerator are simply integers!
And the denominator is a power of two. Thus, by our multiplication by $\frac{1}{2}$ lemma and [[discrete_power_rule]], we have that the derivative of $x^{c_{n}}$ :
$$
c_{n}x^{c_{n} - 1} > 0 \tag{1}
$$
Now we can use the fact that this is [[uniformly_convergent]] in some interval $\left[ \frac{1}{M}, M \right]$ to prove with [differential_by_uniform_convergence] that the general power rule holds:
Consider:
$$
|x^{c_{n}} - x^t| = |x^t(x^{c_{n} - t} - 1)| \leq |M^t(x^{c_{n} - t} - 1)|
$$
Also notice that for each $c_{n}$, the derivative is defined and it is positive (1), so for values higher than $1$ we are interested in the value that is the greatest if we want to be the furthest away from $1$ and for values lower than 1 we are interested in the smallest values and, thus, closer to 0.
So to find the maximum of the difference to the limit of the interval we simply need to grab the ends and, thus, prove that this part is uniformly convergent:
$$
\lim_{ n \to \infty } |c_{n} - t| = 0 \implies \lim_{ n \to \infty } \left\{  M, \frac{1}{M}  \right\}^{c_{n} - t} = 1 \implies \lim_{ n \to \infty } x^{c_{n} - t} = 1
$$
This implies that we simply pick $n \geq N$ :
$$
x^{c_{N} - t} \in \left( 1 - \frac{1}{2\varepsilon M^t}, 1 + \frac{1}{2\varepsilon M^t} \right)
$$
This implies that for $n \geq N$
$$
|M^t(x^{c_{n} - t} - 1)| \leq |M^t \frac{1}{2\varepsilon M^t}| = \frac{1}{2 \varepsilon}
$$
Consequently, the whole is uniformly convergent and, thus, we know that the limit of the derivatives is the derivative of the function that it is moving towards:
$$
\lim_{ n \to \infty } c_{n}x^{c_{n} - 1} = tx^{t - 1}
$$
Any number that is not $0$ can be found in such an interval defined by $M$, thus, we know that any number other than $0$ follows the power rule and we know that $(x^0)' = 0$ which is an exception to the rule as by the rule it should be $x^{-1}$.
Thus, we know that the power rule holds on all of $R$ except $0$ $\square$