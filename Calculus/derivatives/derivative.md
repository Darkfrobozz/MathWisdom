The rate of change, specifically in relation to functions is what we wish to explore.
Let's then suppose we have some function $f$ and wish to analyse the rate of change at some point $x$, a natural response to this would be to analyse what happens when we move some small distance $h$:
$$
f(x + h) = f(x) + ?
$$
One way to approximate this is to make [[linear_approximation]] using a line at the point $x$ for a [[continuity]] [[function]] this makes sense because at some point both the value of the function and the value of the line are very close to the value $f(x)$  and, thus, the error must be very small the closer we get which is what we want.
However, note that the choice of line must be verified whether it is the best approximation, intuitively, a the line that follows the direction of the function is the best line.

Ignoring to analytically prove this for now nets us the derivative, which is basically a calculation to establish a line that follows the curve.
And the notation for the derivative is $f'(x)$:
$$
f'(x) = \lim_{ h \to 0 } \frac{ f(x + h) - f(x)}{h}
$$
Interestingly, the line from this seem to approach the tangent from geometry.