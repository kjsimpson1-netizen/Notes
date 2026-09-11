This is a powerful strategy to solve [[Partial Differential Equations]]. This can be done when the [[Math/Differential Equations/Differential Equations|Differential Equations]] can be broken down into each of it's parts, where we assume that neither of the variables are dependent upon each other, i.e.:
$$
\begin{aligned}
u(x,t)=X(x)T(x)
\end{aligned}
$$
Therefore, when we take the partial derivatives, we get:
$$
\begin{aligned}
u_x&= X'(x)T(t)\\
u_t&= X(x)\dot T(t)
\end{aligned}
$$
From this point, we can plug in the expression into the [[Partial Differential Equations]]. 
## Example of Heat Equation
The heat equation is:
$$
\begin{aligned}
u_t=Du_{xx}
\end{aligned}
$$
With boundary conditions of:
$$
\begin{aligned}
u(x,0)=f(x)\\
u_x(0)=u_x(L)&= 0
\end{aligned}
$$
We can from here plug in the equivalent expressions from above:
$$
\begin{aligned}
\frac{dT}{dt}X&= DT\frac{d^2X}{dx^2}
\end{aligned}
$$
From here, we have that the two derivatives are all equal to a constant, and a [[Strum-Louisville Eigenvalue Problem]], since the equation above states that the rate of change in space is independent of time, and thus a constant. Therefore, we can choose our eigenvalue:
$$
\begin{aligned}
\frac1{TD}\frac{dT(t)}{dt}&= \frac1{X}\frac{d^2X(x)}{dx^2}= -\lambda=-\mu^2
\end{aligned}
$$
>[!Note]
>We could work through the cases where the eigenvalues are positive or 0, but both will lead to trivial solutions. 

We can now solve the two resultant [[Ordinary Differential Equations]]:
### Space Equation
First solving $\frac{dX^2(x)}{dx^2}=-X(x)\mu^2$ gives us the solution $X(x)=A\cos(\mu x)+B\sin(\mu x)$. We can now apply the boundary conditions, which gives us that:
$$
\begin{aligned}
X'(0)&= B\mu=0&&\implies B=0\\
X'(L)&= A\mu\cos(\mu L)=0&&\implies \mu_n=\frac{\pi n}{2L},n\in\mathbb{N}
\end{aligned}
$$
This gives us the eigenvalues, which we can then plug into the solution for $X(x)$:
$$
\begin{aligned}
X_n(x)=A\cos\left(\frac{\pi n}{2L}\right)
\end{aligned}
$$
>[!Note]
>Note the $n$ in the equation here, as any integer value of $n$ will satisfy the eigenvalue.
### Time Equation
This one is easy to solve, as $\frac{dT(t)}T=-\mu^2dt$ has the solution $T_n(t)=\exp(-\mu^2 t)$.
### Putting it together
We can now express the full solution:
$$
\begin{aligned}
u_n(x,t)&= X_n(x)T_n(t)\\
&= c_n\cos(\mu x)\exp(-\mu^2t)\\
&= c_n\cos\left(\frac{\pi n}{2L} x\right)\exp\left(-\left(\frac{\pi n}{2L}\right)^2t\right)
\end{aligned}
$$
The full solution will be the summation of all values of $n$, therefore:
$$
\begin{aligned}
\boxed{u(x,t)= \sum_{n=0}^\infty c_n\cos\left(\frac{\pi n}{2L} x\right)\exp\left(-\left(\frac{\pi n}{2L}\right)^2t\right)}
\end{aligned}
$$
And from here, the values of $c_n$ can be determined via initial conditions. **