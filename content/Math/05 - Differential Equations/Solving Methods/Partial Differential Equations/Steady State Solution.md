For [[Partial Differential Equations|PDE]]'s of the form
$$
\begin{aligned}
u_t=u_{xx}+g(x)
\end{aligned}
$$

We can solve these by finding the steady state. Assume that $\lim_{t\to\infty}u_t=0$, then we have that:
$$
\begin{aligned}
0&= u_{xx}+g(x)
\end{aligned}
$$
Then from here, we can solve this [[Ordinary Differential Equations|ODE]], calling it $u_x(x)$, applying the [[Boundary Conditions]]. We can then express $u(x,t)=u_s(x)+v(x,t)$. Plugging this in:$$
\begin{aligned}
(u_s+v)_t&= (u_s+v)_{xx}+g(x)\\
v_t&= v_{xx}+\cancel{(u_s+g(x))}\\
v_t&= v_{xx}
\end{aligned}
$$
