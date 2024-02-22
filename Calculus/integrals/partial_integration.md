The main purpose of this method is to work with the product of two [[integral]], here we make use of the [[fundamental_thereom_of_calculus]] to assert that the following is true:
$$
\int f(x)g(x) \, dx = F(x)g(x) - \int F(x)g'(x) \, dx  
$$
We can prove this by taking the derivative and applying the [[fundamental_thereom_of_calculus]] to the two integrals.
$$
f(x)g(x) = (F(x)g(x))' - F(x)g'(x)
$$
Recognizing that $F$ is an integral we can use [[product_of_derivatives]] and [[fundamental_thereom_of_calculus]] to confirm that the equation is true.
$$
f(x)g(x) = f(x)g(x) + F(x)g'(x) - F(x)g'(x) = f(x)g(x)
$$