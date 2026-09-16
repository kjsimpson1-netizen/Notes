We will only treat the 2 component case. Given:
$$
\begin{aligned}
\vec f(g,h)=\begin{pmatrix}
f(x,y)\\h(x,y)
\end{pmatrix}
\end{aligned}
$$
We want to find the roots $x^*$ such that $\vec f(\vec x)=0$. We can first find the [[Jacobian Matrix]] of this, which will give:
$$
\begin{aligned}
\mathbb{J}(x)=\begin{pmatrix}
\frac{\partial f}{\partial x}&\frac{\partial f}{\partial y}\\
\frac{\partial g}{\partial x}&\frac{\partial g}{\partial y}
\end{pmatrix}
\end{aligned}
$$
We should also have that $\mathbb{J}(x_*)$ is invertible. We will be able to find the root $x_*$ by taking the [[Tangent Planes]] of $\vec f(x_0)$, where $x_0$ is an initial guess. From this point, we can find the root similar to [[Newton-Raphson Method]]. This will end up solving the system of equations:
$$
\begin{aligned}
\mathbb{J}(x_n)\begin{bmatrix}
x_{n+1}-x_n\\
y_{n+1}-y_n
\end{bmatrix}&= -\begin{bmatrix}
f(x_n,y_n)\\
g(x_n,y_n)
\end{bmatrix}
\end{aligned}
$$
Which has the solution that:
$$
\begin{aligned}
\boxed{\vec x_{n+1}=x_n-\underbrace{\mathbb{J}^{-1}(\vec x_n)\vec f(\vec x_n)}_\delta}
\end{aligned}
$$
