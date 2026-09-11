These are ways to turn [[Open Statements]] into a [[Logical Statements]]. For example: "The number $x^2$ is non-negative" is an [[Open Statements]], however "The number $x^2$ is non-negative for all reals" is a [[Logical Statements]] due to the term "for all reals". This is the quantifier.
## Universal Quantifier
This is the symbol $\forall$ and this adds context to an open statement, and it is read as "for all". To prove this true, we have to prove it for **all** values, however to prove it false we only need **one** counterexample. 
## Existential Quantifier
This is the symbol "$\exists$" and this also adds context, and it is read as "there exists". For this to be true, we only need **one** value and then it is true, however for it to be false  we need to prove it **generically**. 
## Negations
>[!Note]
>Letting $P(x)$ be an [[Open Statements]] over the domain $A$, then the following holds with it's [[Negation]]:
>
>
$
\begin{aligned}
\sim(\forall \in A,P(x))\quad&\equiv\quad\exists \in A\;st\;\sim(P(x))\\
\sim(\exists \in A\;st\;(P(x)))\quad&\equiv\quad\forall \in A,\sim P(x)
\end{aligned}
$
## Nested Quantifiers
In general, qualifiers do not commute and the order matters. We go in order from left to right. 