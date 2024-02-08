## Definition
A compact set $A$ is such a set that any sequence of the set has a convergent subsequence such that:
$$
\lim_{ n \to \infty } (x_{n}) = x
$$
Implies that $x \in A$
## Closed Property
If there exists a sequence and its limit exists then all its subsequence by [[discrete_limits]] converge to that limit as well.
This implies that since this sequence has a convergent subsequence whose limit is in the set.
Then that limit must be in the set. 
Thus, it is a [[closed_set]].

## Bounded Property
If the set has a sequence that is unbounded then we can extract a subsequence of that unbounded sequence such that it is strictly monotone.
If we then pick a subsequence of this set then it must also be monotone and, thus, if it were bounded then the previous sequence discussed could not have been unbounded.
This leads to a contradiction.
Therefore, a compact set is bounded.

## Logical Equivalence
By the [[finding_convergent_subsequences]], we have that a bounded set implies that we can find for all sequences a subsequence that converge. Moreover, by the closed property, we can ascertain that those subsequence on their own are sequences and, thus, their limits must be within the set.
Consequently, we can observe that there is a logical equivalence of these two properties and a compact set.