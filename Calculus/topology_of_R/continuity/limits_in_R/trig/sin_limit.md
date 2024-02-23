To prove the derivative for $\sin$ we will investigate the derivative: 
$$
\lim_{ x \to 0 } \frac{\sin x}{x}
$$
Let's look at the unit circle:
![[unit_circle.png]]
Here we can see that the area of the triangle equals
$$
\sin x \cos x
$$
We can also observe that the area of the $x$ slice of the circle is
$$
x
$$
Assuming $x$ is in radians.

So, we can see that :
$$
\sin x \cos x < x
$$
Now we may also extend the circle :
![[extended_unit.png]]
Now again viewing the areas we can also see that :
$$
x < \tan x = \frac{\sin x}{\cos x}
$$
This then implies that
$$
\sin x \cos x < x < \frac{\sin x}{\cos x} \implies \cos x < \frac{x}{\sin x} < \frac{1}{\cos x} \implies \frac{1}{\cos x} > \frac{\sin x}{x} > \cos x
$$
So we can conclude that by [[squeeze_thereom]]:
$$
\lim_{ x \to 0 } \frac{\sin x}{x} = 1
$$