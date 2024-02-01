## Questions
![[Pasted image 20240201150701.png]]
## Answers
## General
To answer this question we need a thorough understanding of Taylor expansions and polynomial approximations.
First let's make the assumption that there exists some set of constants $A = \{ a_{0}, a_{1}, a_{2} \dots \}$ such that the following is correct:
$$
\sin x = a_{0} +a_{1}x + a_{2}x^2 + a_{3}x^3 \dots \tag{1}
$$
// Note that this assumption is not proven here
However, we can evaluate how good this approximation is by evaluating the error between the approximation and the exact form :
#todo 
- [ ] ⏫ Reference Lagrange here to estimate error.

## Answer to $(a)$
Using $(1)$, we can use the predictable properties of trigonometric and polynomial derivatives to find an answer for the set $A$ around $x = 0$ :
$$
\sin x = a_{0} + \sum_{1}^\infty(a_{n}x^n) \implies \sin 0 = a_{0} \implies a_{0} = 0
$$
We will come back to this tactic of nulling terms by fixing $x = 0$ but to find the rest we must make sure the constant we are trying to find is not multiplied by $x$. Incidentally, the property of polynomial derivation helps in this pursuit :
$$
(\sin x)' = a_{1} + 2a_{2}x + 3a_{3}x^2 + \sum_{4}^\infty na_{n}x^{(n - 1)}
$$
We have now effectively isolated $a_{1}$ and can fix $x = 0$ :
$$
\cos 0 = a_{1} + \dots \implies a_{1} = 1
$$
Continuing this procedure and leaving out subsequent terms for sake of clarity :
$$
(\cos x)' = 2a_{2} + 3 \cdot 2 a_{3}x + \dots \implies -\sin 0 = 2a_{2} \implies a_{2} = 0
$$
$$
(- \sin x)' = 3 \cdot 2 a_{3} + \dots \implies -\cos 0 = 6a_{3} \implies a_{3} = \frac{1}{6}
$$
$$
(- \cos x)' = 4 \cdot 3 \cdot 2 a_{4} + \dots \implies \sin 0 = 24a_{4} \implies a_{4} = 0
$$
Now we were aiming for a polynomial of degree 4 so we may stop here as we have found the constants of the first five terms in $(1)$ :
$$
\sin x \approx x + \frac{1}{6}x^3 \tag{2}
$$
Now we can fix $x = \frac{1}{10}$ :
$$
\sin \frac{1}{10} \approx \frac{1}{10} + \frac{1}{6 \cdot 10 \cdot 10} = \frac{61}{600}
$$
## Answer to $(b)$
#todo 
- [ ] ⏫ Continue answer by calculating using the error formula introduced in general segment 