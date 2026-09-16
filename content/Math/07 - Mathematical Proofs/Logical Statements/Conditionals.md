---
aliases:
  - Implication
---
These are [[Logical Statements]] that takes the form "if P is true/false then Q". This is an implication, and it takes that symbol $\implies$. The order for this statement also matters, and $P\implies Q\neq Q\implies P$. The truth table for this is:

| $P$ | $Q$ | $P\implies Q$ |
| --- | --- | ------------- |
| T   | T   | T             |
| T   | F   | F             |
| F   | T   | T             |
| F   | F   | T             |
This is only false when the implication is true and the conclusion is false. We can also write this using a [[Conjunction]]:
$$
\begin{aligned}
P\implies Q\equiv (\sim P)\lor Q
\end{aligned}
$$

