## Theory
The idea of this technique is taking a fraction and splitting it up into a more approachable format.
Specifically, we are interested in splitting up into the real roots of the polynomial in the denominator.
In particular, since we are only interested in real roots we can at the end either get quadratics or linear expressions.
Moreover, we are only interested in fractions that are of a degree exactly one less than the denominator, this creates a structured format to work with.

## Example
To start with this we need to perform polynomial division :
$$
\frac{x^{2} + 5x + 10}{x^{2} + 5x + 6} = 1 + \frac{4}{x^{2} + 5x + 6}
$$
As a result, we start by factorizing the denominator.
$$
\frac{x^{2} + 5x + 10}{x^{2} + 5x + 6} = \frac{4}{(x+3)(x+2)}
$$
Then to continue we assume that a partial decomposition exists :
$$
\frac{A_{1}}{x + 3} + \frac{A_{2}}{x+ 2} = \frac{4}{(x+3)(x+2)} 
$$
This generates a [[linear_equation_system]] :
$$
A_{1}(x+ 2) + A_{2}(x+3) = 4 
$$
$$
A_{1}x + A_{2}x = 0x \land 3A_{1} + 2A_{2} = 4
$$
To solve this :
$$
\begin{bmatrix}
1 && 1 \\
3 && 2
\end{bmatrix} =
\begin{bmatrix}
0  \\
4
\end{bmatrix}
$$
We simply need to calculate the reverse:
$$
\begin{bmatrix}
1 & 1 & | & 1 & 0 \\
3 & 2 & | & 0 & 1
\end{bmatrix}
=
\begin{bmatrix}
1 & 1 & | & 1 & 0 \\
0 & -1 & | & -3 & 1
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 & | & -2 & 1 \\
0 & -1 & | & -3 & 1
\end{bmatrix}
=
\begin{bmatrix}
1 & 0 & | & -2 & 1 \\
0 & 1 & | & 3 & -1
\end{bmatrix}
$$
So we get the inverse, applying it on both sides we should get the answer :
$$
\begin{bmatrix}
1 && 0 \\
0 && 1
\end{bmatrix}
=
\begin{bmatrix}
0  \\
4
\end{bmatrix}
\begin{bmatrix}
-2 & 1 \\
3 & -1
\end{bmatrix}
=
\begin{bmatrix}
4 \\
-4
\end{bmatrix}
$$
Consequently we have that $A_{1} = 4 \land A_{2} = -4$
Thus, we have our solution and can complete the partial fractional decomposition:
$$
\frac{4}{x + 3} + \frac{-4}{x + 2} = \frac{4}{(x+3) (x+2)}
$$