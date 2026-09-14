We can also solve [[Second Order Differential Equation]] (similar to that of [[Euler Equations]]) however with different powers for the coefficients of $x$ for a more general method. In order to get these equations, we will have to sometimes approximate the solution using [[Taylor Series]]. These are used to solve equations of the form:
$$
\begin{aligned}
P(x)y''+Q(x)y'+R(x)y&= 0&&(1)
\end{aligned}
$$
We replace each of the coefficient equations and each term of $y$ with it's [[Power Series]]. 
>[!Note]
>For each $y$, we replace it with $\sum _{n=0}^{\infty}a_n(x-x_0)^n$. However, if we have the expansion point $x_0$ as a singular point (i.e. non-differentiable), this means that the expansion will not work.

After replacing all of the $y$'s with the respective expressions, we can then multiply all of them by their respective polynomial coefficients. From this point onwards, it is all algebraic solving for the coefficients. 
## Recurrance
When solving this equation, we will always get a value for $a_0$ and $a_1$, and then after this we will have a recurrence
equation which will show how the equation repeats and continues onwards after the initial terms
>[!Note]
>After we have obtained the expressions for the terms of $a_n$, we can write it in a series, replacing all the like terms with the same degree of $a$.  i.e. we take the following:
>$$
\begin{aligned}
>\sum _{n=0}^\infty a_nx^n=a_0+a_1x+a_2x^2...
\end{aligned}
$$
And then replace all the $a_n$th terms with it's valid expression. If the [[Ordinary Differential Equations]] is not [[Homogeneity|Homogenous]], then we just equate to the equivalent degree of $x$ rather than 0.

## Radius of Converge
The [[Radius of Convergence]] of t his series is the range of values of the solution, and we have two ways to find it:
1. We can find the nearest point of the original equation $(1)$ where the coefficient $p(x)=0$, since this will create a [[Singular Point]]. This will give us a lower bound on the [[Radius of Convergence]].
2. We can also use the [[Ratio Test]] of the [[Series Circuits|Series]]. 
>[!Note]
>For ratio test, we must do it in the general case, i.e. with the full expansion of the nth term ($a_{n}x^{n}$) instead of just the coefficient $a_n$.
