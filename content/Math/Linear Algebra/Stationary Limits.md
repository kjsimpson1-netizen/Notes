After a large amount of iterations, a [[Markov Matrix]] will continue to output the same value, or expressed mathematically as:
$$\begin{align*}
P\vec x_s&= \vec x_s
\end{align*}$$
We can find the value for $x_s$ by doing the following:
$$\begin{align*}
&&I\vec x_s-P\vec x_s&= 0\\
&\implies&(I-P)\vec x_s&= 0
\end{align*}$$
We can then substitute in the values for $P$, leaving us with a [[Matrix]] which can be solved using [[Gaussian Elimination]]. 

