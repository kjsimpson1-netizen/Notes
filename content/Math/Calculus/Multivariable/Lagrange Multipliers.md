These are useful tools for solving maximization problems, where we are looking for the global maxima or minima. The function, lets call it $f$, being optimized is called the *objective function*, and the function whose zero set is the curve of interest, call it $g$, is called the constraint function. We can then set up the following system of equations, by equating the two [[Gradient]] of the functions:
$
$
\begin{aligned}
\nabla f(x,y,z)&= \lambda\nabla g(x,y,z)\qquad\lambda\in\mathbb{R}\\
g(x,y,z)&= 0
\end{aligned}
$
$
From this point, we just solve the remaining system of equations.
>[!Note]
>If there is two constraining functions, we can treat this very similarly by solving:
>$
$
\begin{aligned}
\nabla f(x,y,z)= \lambda\nabla g(x,y,z)&+\mu \nabla h(x,y,z)\qquad\lambda,\mu\in\mathbb{R}\\
g(x,y,z)&= 0\\
h(x,y,z)&= 0
\end{aligned}
$
$

