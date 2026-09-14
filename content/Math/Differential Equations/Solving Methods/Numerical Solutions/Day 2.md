## Scalar Root finding
We are looking to find the zeroes of $f(x)$, $f(x_*)=0$. We can do this using either the bisection method or the [[Newton-Raphson Method]], both of these will generate a sequence of approximations, such that as we go further in the sequence, the value will get closer to the true root.
$$\begin{align*}
\lim_{n\to\infty}x_n&= x_*
\end{align*}$$
## Bisection
This method is more general, as we only require that the function here be [[Continuity|Continuous]]. Let $f(x)\in[a,b]$, and $\text{sgn}(f(a))=-\text{sgn}(f(b))$, thus by [[Intermediate Value Theorem]], there must be a 0 somewhere in the interval.
We will first check the midpoint, $x_1=\frac{a+b}2$ and evaluate $\text{sgn}(f(x_1))$. If the sign of $f(x_1)$ if different than $f(a)$, then $x_*\in[a,x_1)$, if it is the same, then $x_*\in(x_1,b]$. 
From here, we repeat with a new midpoint being $x_2=\frac{x_1+a}2$ (depending on whether it was in the right or the left section).
We have that $B_{n+1}=\frac12B_n^1$ for this method. 
>[!Note]
>The $\frac12$ is called the convergence factor, and the $B^1$ represents the order of the method. 

