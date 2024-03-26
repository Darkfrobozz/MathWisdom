The deviation or variation is the goal of measuring that given some average pick what will the offset be. That is how far on average will we be from our average pick.
A natural way to approach this is taking the average of the difference between some average and each element. That is in fact how we calculate variance:
$$
v = \frac{1}{n - 1} \sum_{i=1}^{n}(x_{i} - \bar{x})^2
$$
There are several aspects to explore here such as the reasoning behind squaring when taking the variance is because otherwise it would end up being just 0 but by taking the square, we make each term positive so the variance will add up for each. Moreover, we divide by $n - 1$ instead of $n$, this is because most often we are working with sample instead of a population and, thus, we want an overestimation of deviation rather than underestimation. So, we artificially make the value slightly bigger by dividing by $n - 1$. For populations, we would use $n$.

This variance can then be used to compute standard deviation, which is simply :
$$
\sqrt{ v } = \sqrt{ \frac{1}{n - 1} \sum_{i=1}^{n}(x_{i} - \bar{x})^2 }
$$
This is done because we are trying to counteract the effect of squaring each of the term by retrospectively taking the square root.