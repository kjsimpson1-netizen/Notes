 This is a method to find the solution of a linear [[Ordinary Differential Equations|ODE]] of the form:
$$
\begin{aligned}
\boxed{y'+p(x)y= f(x)}
\end{aligned}
$$
### Integrating Factor
We can solve these by introducing a integrating factor, $r(x)$. This $r(x)$ is chosen such that the derivative is the function $p(x)$ multiplied by an exponential.
$$
\begin{aligned}
r(x)&= e^{\int p(x)dx}\\
\\
\hline\\
\implies r'(x)&= p(x)e^{\int p(x)dx}\\
&= p(x)r(x)
\end{aligned}
$$
This is useful because we can then multiple both of the sides by $r(x)$ to get:
$$
\begin{aligned}
r(x)y'+r(x)p(x)y&= r(x)f(x)
\end{aligned}
$$
And if we look at the left side of the equation, we can see that this can come from the [[Product Rule]]:
$$
\begin{aligned}
\frac d{dx}\Big[r(x)y\Big]&= r'(x)y+y'r(x)\\
&= r(x)p(x)y+y'r(x)
\end{aligned}
$$
### Solving
This is useful because we can then simplify the left side into the form:
$$
\begin{aligned}
\frac d{dx}\Big[r(x)y\Big]&= r(x)f(x)
\end{aligned}
$$
We can now integrate both sides for our answer:
$$
\begin{aligned}
r(x)y&= \int r(x)f(x)dx\\
\implies y&= \frac1{r(x)}\cdot\int r(x)f(x)dx
\end{aligned}
$$
