Given the geometric interpretation of a [[matrix]], we can argue for what should be the product of two matrices. That is what is the transformation that is two known transformations in a sequence.

Using that the first matrix tells us where the standard basis will land we can use a generalization :
$$
\begin{bmatrix}
1 \\
0 \\
. \\
. \\
. \\
0
\end{bmatrix}
\begin{bmatrix}
a_{11} & . & . & . & & & a_{n1} \\
. \\
. \\
. \\ \\

a_{1n} & . & . & . & & & a_{nn}
\end{bmatrix}
\begin{bmatrix}
b_{11} & . & . & . & & & b_{n1} \\
. \\
. \\
. \\ \\

b_{1n} & . & . & . & & & b_{nn}
\end{bmatrix}
$$
Now seeing where the basis vector eventually land we first get that :
$$
\begin{bmatrix}
a_{11} \\
a_{12} \\
. \\
. \\
. \\
a_{1n}
\end{bmatrix}
$$

And since this now consists of standard basis we can see that the standard basis will land at :
$$
\begin{bmatrix}
a_{11}b_{11} + a_{12}b_{21} + \dots + a_{1n}b_{1n}\\
a_{11}b_{21} + a_{12}b_{22} + \dots + a_{1n}b_{2n}\\
. \\
. \\
. \\
a_{11}b_{1n} + a_{12}b_{2n} + \dots a_{1n}b_{nn}
\end{bmatrix}
$$
This is then the first matrix of the resultant matrix since that is where the standard basis landed.

Consequently, the [[matrix]] product is similar to the [[vector_dot_product]] of matching components :
$$
\begin{bmatrix}
0 & 1 \\
5 & 1
\end{bmatrix}
\begin{bmatrix}
5 & 3 \\
6 & 2
\end{bmatrix} =
\begin{bmatrix}
6 & 2 \\
28 & 17
\end{bmatrix}
$$
Here we can see that we take the vector product :
$$
\begin{bmatrix}
0 & 1
\end{bmatrix}
\begin{bmatrix}
5 \\
6
\end{bmatrix} 
$$
To get index 0, 0 of the resulting matrix.

This kind of product results in a specific requirement that the first matrix must have the same amount of columns as the second matrix has rows.
And the columns of the second decides the resultant columns, similarly, the rows of the first is the rows of the result.