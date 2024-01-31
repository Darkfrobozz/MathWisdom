Consider the [[derivative]] for $f, g$ and, then, what could the [[derivative]] of $f \cdot g$ be?
$P_{1}$ is:
$$
(f \cdot g)' = f'g + g'f
$$
Now this differs greatly from [[product_of_limits]] but we will still use the limit definition and [[product_of_limits]] to prove it:
$$
(f \cdot g)' = \lim_{ h \to 0 } \frac{f(x+h)\cdot g(x+h) - f(x)\cdot g(x)}{h} = \lim_{ h \to 0 } \frac{f(x+h) \cdot g(x+h) - f(x+h)g(x) + f(x+h)g(x) - f(x)g(x)}{h}
$$
Now we can split this using [[product_of_limits]]
$$
(f\cdot g)' = \lim_{ h \to 0 } \frac{f(x +h)(g(x+h) - g(x)) + g(x)(f(x+h) - f(x))}{h} = \lim_{ h \to 0 } f(x+h)\frac{g(x+h) - g(x)}{h} + \lim_{ h \to 0 } g(x)\frac{f(x+h) - f(x)}{h}
$$
That looks awfully familiar no?
It is, using [[sum_of_limits]] we can split this even further to complete the proof:
$$
\lim_{ h \to 0 } f(x+h) \lim_{ h \to 0 } \frac{g(x+h) - g(x)}{h} + \lim_{ h \to 0 } g(x) \lim_{ h \to 0 }\frac{(f(x+h) - f(x))}{h} 
$$
Now we can just compute these limits leaving us with $P_{1}$.