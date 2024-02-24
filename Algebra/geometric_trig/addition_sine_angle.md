We want to understand what happens to our trig functions when we add angles.
For example, $\sin(x+y)$ and $\cos(x+y)$ :
![[additive_angles.png]]
Notice that we start with $1$ here and what we need to find now is the relation between the hypotenuse and the opposite and adjacent to the angle $x+y$.

To prove this we start by using sine and cos :
![[additive_angles2.png]]
Here we can notice that we have some similar right triangles and we will establish some key lengths by ratios:
![[additive_angles4.png]]
$$
\frac{\frac{\sin x}{\cos x}}{\frac{1}{\cos x}} = \frac{R_{1}}{1} \implies R_{1} = \sin x
$$
$$
\frac{\sin x}{\frac{1}{\cos x}} = \frac{R_{2}}{1} = \sin x \cos x
$$
$$
\frac{\sin x \cos x}{\cos y} = \frac{R_{3}}{1} = R_{3}
$$
$$
\frac{R_{4}}{\frac{\sin x}{\cos x}} = \sin x \cos x = \sin^2 x
$$
$$
\frac{R_{5}}{\sin y} = \frac{\sin x \cos x}{\cos y} = \frac{\sin x \cos x \sin y}{\cos y}
$$
$$
R_{6} = 1 - \sin^2 x - \frac{\sin x \cos x \sin y}{\cos y} = \cos^2x - \frac{\sin x \cos x \sin y}{\cos y}
$$
$$
\frac{R_{7}}{\sin y} = \cos^2x - \frac{\sin x \cos x \sin y}{\cos y} = \cos^2 x \sin y - \frac{\sin x \cos x \sin^2 y}{\cos y}
$$
$$
R_{8} = \frac{\sin x \cos x}{\cos y} + \cos^2 x \sin y - \frac{\sin x \cos x \sin^2 y}{\cos y}
$$

$$
R_{8} = \sin(x+y) \cos x \implies \sin (x+y) = \frac{\sin x}{\cos y} + \cos x \sin y - \frac{\sin x \sin^2 y}{\cos y}
$$
$$
R_{9} = \frac{\sin x \cos x}{\sin x} = \cos x
$$
![[additive_angles3.png]]

$$
(\sin x) \frac{1 - \sin^2 y}{\cos y} = \sin x \cos y
$$
$$
\sin(x+y) = \cos x \sin y + \sin x \cos y
$$