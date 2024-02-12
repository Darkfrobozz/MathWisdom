First, we take our [[function]] $f$ that has [[continuity]] and defined on the [[domain]] $A$ and produces the [[range]] $B$:
$$
f : A \to B
$$
We then want to prove that if $A$ is a [[compact_set]], then $B$ is also a [[compact_set]].
To prove this, we take a sequence from $B$ :
$$
(b_{n}) \in B
$$
Since this is the [[range]] of a [[function]] we know that there exists some sequence $a_{n}$ such that $f(a_{n}) = b_{n}$ and using this and that $A$ is a [[compact_set]] we can produce a subsequence of $(a_{n}) : (a_{n_{1}})$ such that it converges to $a \in A$ :
Then it is clear that we can map this sequence with $f$ to $B$.
Consequently, since we know that the [[function]] has [[continuity]] at all points in the [[domain]] it also has to have this on $a$ which means that since $a_{n_{1}}$ converges to $a$ :
$$
\lim_{ n \to \infty } f(a_{n_{1}}) = f(a)
$$
And since we started with that these points were taken from a sequence in $B$, we can conclude that there existed a subsequence of $(b_{n})$ such that it converged to a value in $B$. $\square$