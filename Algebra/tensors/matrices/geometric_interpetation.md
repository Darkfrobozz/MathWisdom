# Introduction
We are interested in equations :
$$
b = Ax
$$
$A$ is here some matrix that maps $x$ to $b$ :

# Standard Basis
Let's consider the standard basis of some vector space.
These by definition will have linear combinations that span that vector space.

# Relation to Matrice
We can now observe that if we multiply :
$$
\begin{bmatrix}
1 & 2 & 0 \\
-5 & 3 & 1
\end{bmatrix}
\begin{bmatrix}
1 \\
0 \\
0
\end{bmatrix} = 
\begin{bmatrix}
1 \\
-5
\end{bmatrix}
$$
Then we see where the standard basis is located in when mapping from $R^3$ to $R^2$
Thus, we can correctly identify that a matrix's columns simply tells us where the standard basis land.
This remapping of the basis to other vectors shows us a proof of the linearity as we will always stay within the span of the new vectors?

The hallmark of this linearity is that evenly spaced points are evenly spaced after transformation.

# Diagonal Matrix
If we use the concept that a matrix tells us where the basis vector lands, a diagonal matrix of size $n$ such as:
$$
\begin{bmatrix}
\alpha_{1} & & & & &\\
& \alpha_{2} \\
& & . \\
& & & . \\
& & & & . \\
& & & &  & \alpha_{n}
\end{bmatrix}
$$
Tells us that each standard basis is simply scaled in some direction, a scalar transformation of the standard basis vectors.

# Shearing
In this scenario, we fix the parallel property of the sides and simply slide them.
![[x_shear.jpg]]
This can be thought of as choosing a line and sliding the object across that line as a railway :
![[railwaytransformation.png]]
We can slide the upper part of this rectangle across the railway to shear it, railway line transformation!

Since we can think of lines as just a point and its linear combinations with vectors, we can see that shearing in a matrix equates to :
$$
\begin{bmatrix}
\alpha_{1} & \beta & & & &\\
& \alpha_{2} \\
& & . \\
& & & . \\
& & & & . \\
& & & &  & \alpha_{n}
\end{bmatrix}
$$
Here the second basis is now mapped to another point following the railway produced by taking the point the basis first landed on and using the standard basis :
$$
x
\begin{bmatrix}
1 \\
0 \\
0 \\
0 \\
0
\end{bmatrix}
$$
To describe a railway line to move the side upon.

# Orthogonal Matrix
To analyze a orthogonal matrix, we first define it as a system in which the basis vectors are all orthogonal to each other:
![[2D_orthogonal_system.png]]
We then realize that we can use the [[vector_dot_product]] to establish important properties of the orthogonal matrix :
![[dotprod.png]]
Using the property that orthogonal vectors when projected onto each other results in an absolute length of 0, we know that the [[vector_dot_product]] is 0 between all the elements of an orthogonal matrix.

Now since that is true we can [[transponse]] the matrix and using [[matrix_product]] between it and its transposition get the [[identity_matrix]].

The following properties can be derived, that the following is preserved over transformation:
- Angle
- Length
- Area
