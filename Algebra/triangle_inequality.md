The triangle inequality is a statement about the [[absolute_values]] of any number.

## Lemma 1
The sum of two sides of a triangle must be bigger or equal to the third side.
## Lemma 2
Any numbers can be represented in a geometrical sense and the distance to the origin is the [[absolute_values]] of those numbers.
## Triangle Inequality Proof
Using lemma 2 we can construct three points: A, B, C of any numbers *x*, *y*, *z*, respectively.

Moreover, we know that we can find a vector for the distance between two points; e.g. A, B by $A - B = x - y$.

Thus, we know that the distance can be found by:
$$
|x - y| = \bar{AB}, |y - z| = \bar{BC}, |x - z| = \bar{CA}
$$
Now using that these sides are connected (x to y to z to x) and, thus, form a triangle, we can use lemma 1 to prove that:
$$
|x - y| + |y - z| \geq |x - z|
$$
Which is the triangle inequality, the figure below is a representation of this:
![[triangle_identity_figure_1.png]]