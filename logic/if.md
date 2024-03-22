The 'if' statement can be used to discharge assumptions. This can be particularly useful if we have an assumption that is sometimes true and sometimes not.

The format is:
if ... then ...

Where the first ... represent the assumption and the second what is the conclusion based on that assumption. Thus, an if statement takes the shape of a smaller [[proof]] or sequent.
However, a sequent contains only its non discharged assumptions! Which means the assumptions for a sequent are to be substantiated through lemmas or axioms.

We have the sequent introduction rule for this, which is that:
$$
\Gamma \cup \{ o \} \vdash w \implies \Gamma \vdash (o \to w)
$$
The second important sequent is that:
$$
\Gamma \vdash o \land \Delta \vdash (o \to w) \implies
\Gamma \cup \Delta \vdash w
$$
