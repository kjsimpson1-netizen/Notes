## Vector Root Finding
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
## Non-linear Optimization
For a scalar function, $f(\vec x),\vec x\in\mathbb{R}^N$, we have to find roots of the gradient, or $\nabla f(\vec x_*)=0$ in order to find the extrema. In order to find this, we can use the [[Hessian Matrix]].
>[!Note]
>For very large [[Matrix|Matrices]], a method called gradient descent can be used. 

This will use the following model:
$$
\begin{aligned}
x_{n+1}=x_n-l\nabla f(\vec x_n)
\end{aligned}
$$
Where $l$ is called the heuristic, or the learning rate. This is strictly a computational parameter, and is not related to the problem. 
## Interpolation
Functions defined on $[a,b]$. The $\mathcal{C}$ space of continuous functions:
$$
\begin{aligned}
||f||_\infty=\max_{x\in[a,b]}|f(x)|
\end{aligned}
$$
There are subsets of $\mathcal{C}$, such as $\mathcal{C}_n$, where $n$ denotes the number of continuous derivatives. 
$$
\begin{aligned}
||f||_{\mathcal{C}_n}&= \sum_{i=0}^n||f^{(i)}||_\infty
\end{aligned}
$$
