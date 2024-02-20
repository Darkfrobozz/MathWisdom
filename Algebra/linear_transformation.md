A linear transformation is specifically designed to work well with addition and multiplication.
Specifically for the [[field]] $F$, a linear transformation is a [[function]] subset of:
$$
T : F^{n} \to F^{m}
$$
They are defined to satisfy the following :
$$
\begin{align}

& 1. \ \ \ \forall c \in F : \forall \vec{x} \in F^{n} : cT(\vec{x}) = T(c\vec{x})\\
& 2. \ \ \ \forall \vec{x}, \vec{y} \in F^{n} : T(\vec{x}) + T(\vec{y}) = T(\vec{x} + \vec{y})\\
\end{align}
$$
Basically, this implies that scalar multiplication and addition is conserved.
Thinking about this geometrically we can think of three points, say that these are equidistant from each other than what does that imply about their respective mapping.
Well :
$$
\forall \vec{x},\vec{y},\vec{z} : \vec{x} - \vec{y} = \vec{x} - \vec{z} : T(\vec{x} - \vec{y} - (\vec{x} - \vec{z})) = T(0) = \vec{0} = T(\vec{x} - \vec{y}) - T(\vec{x} - \vec{z}) \implies T(\vec{x} - \vec{y}) = T(\vec{x} - \vec{z})
$$
Which means that a linear transformation geometrically means that all points that are equally spaced must be equally spaced after the transformation.