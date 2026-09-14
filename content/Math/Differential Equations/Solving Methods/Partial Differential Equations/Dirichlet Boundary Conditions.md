This is a numerical approximation solution for the 
## Setting it up
For the space, we divide the space up following, $x\in[0,L]$, we divide the interval into $N+1$ evenly spaced points with spaces $\Delta x$. so $x_n=n\Delta x, n\in[0,N]$. 
For the time, we divide it up into intervals such that $t\in[0,T]$ into $M+1$ even spaces, with spaces $\Delta t$ so that $t_k=k\Delta t,k\in[0,M]$. We can now substitute this into the [[Forward Difference Method]]
$$
\begin{aligned}
u_n^{k+1}&= u_n^k+\alpha^2\left(\frac{\Delta t}{\Delta x^2}\right)(u_{n+1}^k-2u_n^k+u_{n-1}^k)
\end{aligned}
$$
Where the exterior most points are determined using [[Boundary Conditions]].
## Ghost Nodes
Since sometimes the equation above will give us nodes outside of our bounds, we can replace the ghost node with:
$$
\begin{aligned}
u_{-1}^k=-2c\Delta x+u_1^k
\end{aligned}
$$
## Example - Solving the Heat Equation
Solve using the finite difference method with the boundary conditions
- $v_n^0=\cos(\frac{\pi n\Delta x}{2}),n\in\mathbb{Z}^+$,
- $v_n^k=0,k\in\mathbb{Z}^+$, 
- $v(1,t)=0$, 
- and $v_x(0,t)=0$.
Solving again for the general form of the heat equation solution using the substitutions:
$$
\begin{aligned}
v_t&= \mu v_{xx}\\
 \frac{v(x_1)t+\Delta x}{\Delta t}&= \mu\frac{v(x+\Delta x_1t)-2v(x_1t)+v(x-\Delta x_1t)}{\Delta x^2}\\
\end{aligned}
$$
>[!Note]
We always use the [[Forward Difference Method]] for the time difference and for the second derivative in space. However, for the space in this equation, we will use the [[Central Difference Method]] for the [[Boundary Conditions]]

In the equation above, we can take $t=t_k$ and $x=x_n$ in order to obtain:
$$
\begin{aligned}
\frac{v_n^{k+1}-v_n^{k}}{\Delta t}=\mu\frac{v_{n+1}^{k}-2v_n^k+v_{n-1{^k}}}{\Delta x^2}
\end{aligned}
$$
Multiplying both sides by $\Delta t$:
$$
\begin{aligned}
{v_n^{k+1}-v_n^{k}}&=\mu(\frac{\Delta t}{\Delta x^2}({v_{n+1}^{k}-2v_n^k+v_{n-1{^k}}}{\Delta x^2})\\
v_n^{k+1}&=v_n^{k}+\mu\frac{\Delta t}{\Delta x^2}({v_{n+1}^{k}-2v_n^k+v_{n-1{^k}}})&(1.7)
\end{aligned}
$$
We can then evaluate this at $n=0$ to get $v_n^{k+1}$:
$$
\begin{aligned}
v_0^{k+1}&=v_0^k+\mu\frac{\Delta t}{\Delta x^2} (v_1^k-2v_0^k+v_{-1}^k)
\end{aligned}
$$
For the initial conditions for this problem, we have that $v_x(0,t)=0$, which we can use the [[Central Difference Method]] to get:
$$
\begin{aligned}
\frac{v_1^k-v_{-1}^k}{2\Delta x}&= 0\\
\implies v^k_1&= v^k_{-1}
\end{aligned}
$$
Thus, we can replace $v_{-1}^k$ with $v_{1}^k$:
$$
\begin{aligned}
v_0^{k+1}&=v_0^k+\mu\frac{\Delta t}{\Delta x^2} (2v_1^k-2v_0^k)
\end{aligned}
$$
