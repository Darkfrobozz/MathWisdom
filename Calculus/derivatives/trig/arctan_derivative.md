To establish the derivative of $\tan^{-1} (x)$ we can think of $x = \tan(y)$
Now we can use [[sin_derivative]], [[cos_derivative]], [[product_of_derivatives]] and [[power_rule]] to find the derivative:
$$
(\tan x)' = \sin x \cdot \frac{1}{\cos x} = \sin x \left( - \frac{1}{\cos^2 x}(-\sin x) \right) + 1 = \frac{\sin^2x}{\cos^2x} + 1 = \frac{1}{\cos^2 x} 
$$
Then we can use [[implicit_derivative]] and [[chain_rule]] to find that:
$$
1 = \frac{1}{\cos^2 y}y' \implies \cos^2 y = y'
$$
Finally we can solve this by using [[tan_relation]] :
$$
\cos y = \frac{1}{\sqrt{ 1 + \tan^2y }} \implies \cos^2y = \frac{1}{1 + \tan^2y} = y' = \frac{1}{1 + x^2}
$$