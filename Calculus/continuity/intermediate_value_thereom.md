The proposition $P_{1}$ of the intermediate value theorem is that if we have a continuous function $f$ on the domain $[a,b]$ and with the range (f(a),f(b)).
Then, for every value $x \in (f(a), (f(b)) : \exists c \in (a,b) : f(c) = x$
Effectively, there exists an intermediate value.

We start this proof by constructing a set from the picking a value $k \in [f(a), f(b)]$ :
$$
\{x \in [a,b] : f(x) < k\}
$$
By [[axiom_of_completeness]], this set has a least upper bound, call it $S$
If we pick any of the endpoints call it $l \in \{ a, b \}$, we can reason for two cases either $f(S) = f(l) \lor f(S) \neq f(l)$, if the former, then we are done. If the latter we can enforce that it is a strict equality and, thus, determine that :
$$
\exists\varepsilon : |f(l) - f(S)| > \varepsilon
$$
But since we can find by [[continuity]] a value that is closer to $S$, we know that $S$ cannot be the least upper bound. So, any of the end points for case two is contradictory.

Now we work under the assumption that $S \in (a,b)$ :
Fixing $S$, we have by [[continuity]] that we can always get closer to $f(S)$ by getting closer $S$.
Moreover, we have that $S$ is a least upper bound :

As we come closer from the right, all values will always be bigger than $f(k)$.
AND
As we come closer from the left, all values will always be smaller than $f(k)$.

This means that since these values exists by [[continuity]] and that they squeeze $S$ by it being a least upper bound that $S$ must map to $k$ through $f$.

Consequently, we proved that for both cases : $\exists c = S : f(c) = k \implies P_{1}$ $\square$
