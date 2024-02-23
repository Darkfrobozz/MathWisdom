We are looking to find what  is :
$$
\lim_{ h \to 0 } \frac{\sin (x + h) - \sin (x)}{h}
$$
First we can use [[sum_of_angles_sin]] to show that this equals:
$$
\lim_{ h \to 0 } \frac{\sin x \cos h + \sin h \cos x - \sin x}{h} = \lim_{ h \to 0 } \frac{\sin h \cos x}{h} + \frac{(\sin x)(\cos h - 1)}{h}
$$
We can use [[sum_of_limits]] and [[sin_limit]] to extract the first part :
$$
\cos x + \sin x \lim_{ h \to 0 } \frac{\cos h - 1}{h}
$$
Similarily, we can use [[cos_limit]] to extract the second part:
$$
\cos x + \sin x \cdot 0 = \cos x + 0 = \cos x
$$
Thus we have that the derivative is $\cos x$