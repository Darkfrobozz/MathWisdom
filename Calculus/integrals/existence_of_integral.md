The proposition is that over a function with [[continuity]] defined on some interval $[a,b]$ there exists an [[integral]] in respect to small changes in $x$ and the summation of the small slices produced by this change and $f(x)$.

To prove this proposition we will create an almost perfect [[partition]] of $[a,b]$, as the set $P_{n}$
This partition is meant to evenly divide the interval $[a,b]$ over $n$ subsets.
Its elements will look like :
$p_{1} = [a, x_{1}], p_{2} = [x_{1}, x_{2}], p_{3} = [x_{2}, x_{3}]$
Such that $|p_{i}| = \frac{a-b}{n}$
Now we know that there exists in each of these by [[existence_of_extremum]] a maximum $M_{i}$ and minimum $m_{i}$.
Thus, we form two series :
$$
U_{n} = \frac{a-b}{n}\sum_{i=1}^{n}M_{i}
$$
$$
L_{n} = \frac{a-b}{n}\sum_{i=1}^{n}m_{i}
$$
The actual area under $f(x)$ must be smaller than $U_{n}$ and bigger than $L_{n}$ since we are taking for each subset interval the extreme estimates for the width.
Now to complete this proof we simply need to observe that by [[intermediate_value_thereom]], we have that in each of these sets a value $m_{i}< k_{i} < M_{i}$ such that $k_{i} \frac{a - b}{n}$ perfectly captures the area under $f(x)$ :
Consequently, we have that this is true for all $n$, we can find a value that perfectly captures the area and we also know that :
$$
\lim_{ n \to \infty } \frac{a-b}{n} = 0 \implies \lim_{ n \to \infty } x_{i} = k_{i} \implies \lim_{ n \to \infty } L_{n} = \lim_{ n \to \infty } U_{n} = \int_{a}^b f(x) \, dx 
$$
This means that if we only continue making the [[partition]]s smaller and smaller, the limit will be the integral.
Thus, we have proven that the integral exists.