
Using [[addition_sine_angle]], $\sin(x+y)$, we can find $\cos (x + y)$ by the [[sin_cos_relation]] :
$$
\sqrt{ 1 - (\cos x \sin y + \sin x \cos y)^2 }
= \sqrt{ 1 - \cos^2 x \sin^2 y - 2 \sin x \cos y \cos x \sin y - \sin^2 x \cos^2 y  }
$$
$$
\begin{align}
& \sqrt{ 1 - \cos^2 x \sin^2 y - 2 \sin x \cos y \cos x \sin y - \sin^2 x \cos^2 y  } \\ \\
& =\sqrt{ \cos^2x - \cos^2 x \sin^2 y + \sin^2x - \sin^2x \cos^2 y - 2\dots } \\
& = \sqrt{ \cos^2x\cos^2y + \sin^2x\sin^2y - 2\sin x \cos y \cos x \sin y } \\
& = \sqrt{ (\cos x \cos y - \sin x \sin y)^2 } \\
& = \pm(\cos x \cos y - \sin x \sin y)
\end{align}
$$
Notice that $\sin x\sin y - \cos x \cos y$ is also an solution to this. However, by putting $y = 0 \land x = 0$, we get that:
$$
\cos(0 + 0) = 0 - 1 \lor 1 - 0
$$
and obviously,
$$
\cos(0) = 1
$$
This implies that the correct answer is :
$$
\cos x \cos y - \sin x \sin y
$$