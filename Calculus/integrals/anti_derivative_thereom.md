# Proposition
The proposition is that given the existence of any integral $F$ of a function $f$:
$$
\int f \, dx = F \implies F' = f
$$
# Proof
To prove this, regard the definition of an [[integral]] and notice that we are concerned with the process of generating more and more accurate series and exploring what the limit of those accurate series are.

For any function $f$ we have that $F$ over $dx$ represents the actually value of the area over $dx$. One way to connect these two is to estimate the area with $f$ :
$$
f(x) \cdot dx + (f(x + dx) - f(x)) \cdot dx\approx F(x + dx) - F(x)
$$
$$
f(x + dx) = \frac{F(x + dx) - F(x)}{dx}
$$
Now this obviously gets more and more accurate, the lesser the change in $F(x)$, the smaller the error will be since the error is in the:
$$
(f(x + dx) - f(x)) \cdot dx
$$
and $f$ has [[continuity]] and, thus, $f(x+dx) - f(x) \to 0$.
Thus, we have that:
$$
\lim_{ dx \to 0 } \frac{F(x+dx) - F(x)}{dx} = \lim_{ dx \to 0 } f(x+dx)
$$
This means that :
$$
F'(x) = f(x)
$$