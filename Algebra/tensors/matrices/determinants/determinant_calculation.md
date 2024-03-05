To calculate the determinant, what we need to do is make use of [[determinant_operations]] and realize that the components of a matrix area simply scaled additions of the unit vectors.
Namely, we could represent the area as produced by the two columns:
$$
A(a\hat{i} + b\hat{j}, c\hat{i} + d\hat{j})
$$
Then using [[determinant_operations]] we can start simplifying this:
$$
\begin{align}

&A(a\hat{i} + b\hat{j}, c\hat{i} + d\hat{j}) \\
&= A(a\hat{i}, c\hat{i} + d\hat{j}) + A(b\hat{j}, c\hat{i} + d\hat{j}) \\
&= A(a\hat{i}, c\hat{i}) + A(a\hat{i},d\hat{j}) + A(b\hat{j}, c\hat{i})+ A(b\hat{j},d\hat{j}) \\
&= 0 + adA(\hat{i},\hat{j}) + bcA(\hat{j}, \hat{i}) + 0 \\
&= ad - bc
\end{align}
$$