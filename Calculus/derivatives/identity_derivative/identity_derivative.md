Of particular usefulness would be a non zero derivative that is equal to itself. In particular, the following should be true:
$$
f(x) = f'(x)
$$
Which means that:
$$
f(x) = \lim_{ h \to 0 }  \frac{f(x+h) - f(x)}{h}
$$
We will narrow our search by making the hypothesis that there exists some constant $c$ for which $f(x) = c^x$
Then we can see that:
$$
c^x 
= \lim_{ h \to 0 } \frac{c^{x+h} - c^x}{h} 
= \lim_{ h \to 0 } c^x\frac{c^{h} - 1}{h} 
\implies
1 = \lim_{ h \to 0 } \frac{c^{h} - 1}{h} 
$$
Now we can place a limit on the other side as well and use [[product_of_limits]]
$$
\lim_{ h \to 0 } h + 1 = \lim_{ h \to 0 } c^h
$$
Then, we can use [[power_of_limits]] to move the final part :
$$
\lim_{ h \to 0 } (h+1)^{1/h} = c
$$
This constant is called $e$ and has the desired property by definition.