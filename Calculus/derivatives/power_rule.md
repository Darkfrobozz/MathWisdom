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