This is another method for solving an [[Ordinary Differential Equations|ODE]]. This is very similar to [[U-Substitution]] for taking an [[Antiderivative]]. An example of this is:
$$\begin{align*}
\frac{dy}{dx}&= (x-y+1)^2
\end{align*}$$
Since this equation is neither separable or linear, we have to use a substitution:
$$\begin{align*}
v&= x-y+1\\
\frac{dv}{dx}&= 1-\frac{dy}{dx}
\end{align*}$$
We can now replace this into the equation to give us something easier to solve:
$$\begin{align*}
1-\frac{dv}{dx}&= v^2
\end{align*}$$
This can now be solved by the method for [[Separable Equations]]. Also much like [[U-Substitution]], after the substitution is done, we can back substitute for the solution. 