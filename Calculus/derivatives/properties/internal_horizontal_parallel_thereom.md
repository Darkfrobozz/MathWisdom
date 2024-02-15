An interesting [[derivative]] is the following :
![[rolle'sthereom.png]]
Here we can see that we have two roots, for illustrative purposes we will call the left root $a$ and the right root $b$ :
Notice that $a - b = 0$ which implies that the line through the two points has slope $0$ and in this case we have that there is a horizontal parallel derivative to that line.
We want to prove that is true in the general case :
First unbind the values $a, b$ and simply make them the most general case where the derivable function between these two $f$ maps both $a$ and $b$ to the same value.
$$
f(a) = f(b) \land a < b
$$
Then there exists in between these a point such that the derivative is :
$$
f'(c) = 0
$$
We know that $f'(x)$ is differentiable, we also know that $f(x)$ has [[continuity]] which implies the [[existence_of_extremum]].
However, if $f(a)$ is both the maximum and minimum then all points must equal $f(a)$ since the existence of another point would become a minimum or maximum.
This then implies that $f : [a,b] \to f(a)$ which means that the slope is $0$ and, if $f(a)$ is not the maximum or not the minimum then that implies the existence of an internal extremum $c$ and by [[derivative_at_internal_extremum]], we know that $f'(c) = 0$
Consequently, there must exist some point in $(a,b)$ such that the derivative is parallel to the horizontal axis.