This number describes the magnitude of the change to the final condition given to by small perturbation in the initial conditions. This is denoted by $\text{cond}(A)$ where $A$ is a [[Matrix]]. The condition number is given by the expression:
$$
\begin{aligned}
\text{cond}(A)&= ||A||\;||A^{-1}||
\end{aligned}
$$
We can also find this from taking the quotient of the largest change to the smallest change of a [[unit vector]], i.e.:
$$
\begin{aligned}
\text{cond}(A)=\frac{\text{Largest Change}}{\text{Smallest Change}}
\end{aligned}
$$
Therefore we can say that $\text{cond}(A)\in[1,\infty)$.