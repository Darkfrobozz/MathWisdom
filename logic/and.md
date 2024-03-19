One of the most basic components of [[proof]]s is the and operator:
$$
\land
$$
The least implicative way to use this is with parenthesis:
$$
(P_{1} \land P_{2})
$$
This is true if both $P_{1}$ and $P_{2}$ are true.

It's relation to [[proof]]s are evident in its sequent application:
$$
(\Gamma \vdash o) \land (\Delta \vdash w) \implies ((\Gamma \cup \Delta) \vdash (o \land w))
$$
In other words, and allows us to piece together two proofs to prove something new.