In 2d, we generalize to the cross product of two vectors as simply the [[determinant]].

However, the cross product is technically not defined in 2D but rather starts in 3D, it still defines the 2D [[determinant]] so to say as it equals a vector that has a length equal to the area of the parallelogram spanned by those two vectors.

We can use the righthand rule to figure out where the cross product is going. Looking at your pointer of right hand and going counter clockwise. 

To compute this we do the following:
$$
\det \left( \begin{bmatrix}
\hat{i} & v_{1} & w_{1}\\
\hat{j} & v_{2} & w_{2}\\
\hat{l} & v_{3} & w_{3}
\end{bmatrix} \right)
$$
To prove this we construct a function:
$$
f(\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}) =
\det \left( \begin{bmatrix}
x & v_{1} & w_{1}\\
y & v_{2} & w_{2}\\
z & v_{3} & w_{3}
\end{bmatrix} \right)
$$
This is a mapping between a variable and the volume produced by it and two constant vectors.
First note that the volume is only proportional to the projection of the variable vector onto the line that is perpendicular to the constant vectors.

We have to prove that it is linear. Thus, we have to prove that:
$$
f(\gamma \begin{bmatrix}
x \\
y \\
z
\end{bmatrix}) = 
\gamma f(\begin{bmatrix}
x \\
y \\
z
\end{bmatrix})
$$
But this is simply the scaling of one of the vectors of the [[determinant]]:
$$

\det \left( \begin{bmatrix}
\gamma x & v_{1} & w_{1}\\
\gamma y & v_{2} & w_{2}\\
\gamma z & v_{3} & w_{3}
\end{bmatrix} \right)
=
\gamma
\det \left( \begin{bmatrix}
x & v_{1} & w_{1}\\
y & v_{2} & w_{2}\\
z & v_{3} & w_{3}
\end{bmatrix} \right)
$$
Moreover, we want to prove that
$$
f( \begin{bmatrix}
x_{1} \\
y_{1} \\
z_{1}
\end{bmatrix} +
\begin{bmatrix}
x_{2} \\
y_{2} \\
z_{2}
\end{bmatrix}) = 

f( \begin{bmatrix}
x_{1} \\
y_{1} \\
z_{1}
\end{bmatrix}) +
f(\begin{bmatrix}
x_{2} \\
y_{2} \\
z_{2}
\end{bmatrix}) = 
$$
Again since the [[determinant]] is [[distrubitive]] when adding a vector to a column, we have that this is also true.

Now we know that it is linear and, thus, we know that it has some [[dual_vector]] that represents the transformation. Which means that there is some [[vector_dot_product]] such that:
$$
\begin{bmatrix}
a_{1} \\
a_{2} \\
a_{3}
\end{bmatrix} \cdot
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
= f(\begin{bmatrix}
x \\
y \\
z
\end{bmatrix})
$$
Thus, we know that we are to look for some vector that if we project onto it we have get the volume of the parallelopipied.
However, as noted only the projection onto the line perpendicular affects the volume so having a vector not parallel to this line would mean that we could infinitely extend in the perpendicular part of that vector to said line and still get an infinite volume, which is a contradiction since that should not affect the volume.
Consequently, we know that this unknown must be parallel to the line of the perpendicular. However, we also know that if the projection of the variable part is the vector 1 onto this part then the volume should be equal to the value of the area and the dot product should result in the mystery vector.
Thus, we can conclude that they are equal!
Moreover, since we can organize the calculation of the determinant to be a linear combination of the variable part we know by the equality what the coordinates of the mystery vector must be.