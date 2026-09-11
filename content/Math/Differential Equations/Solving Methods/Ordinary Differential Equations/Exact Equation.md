   These take the form:
$$\begin{align*}
M(x,y)+N(x,y)\frac{dy}{dx}&=  0\\
\hline\\
M(x,y)&= \frac{\partial f}{\partial y}\\
N(x,y)&= \frac{\partial f}{\partial x}
\end{align*}$$
>[!Theorem]
>For a $F(x,y)$, being the solution to the [[Ordinary Differential Equations|ODE]], to exist, we need to satisfy:
>$$\begin{align*}
\frac{\partial M(x,y)}{\partial y}=\frac{\partial N(x,y)}{\partial x}
\end{align*}$$

## Theorem Holds
If the above theorem holds, we can then solve via taking the [[Antiderivative]] with respect to each variable:
$$\begin{align*}
F(x,y)&= \int M(x,y)\partial x+h(y) 
\end{align*}$$
>[!Warning]
>When taking the [[Antiderivative]], we have to place a function of the opposite variable on the end of the antiderivative.

From that point, we can compare the $N(x,y)$ to $\frac{\partial F}{\partial y}$, and the difference between these two will give us $h(y)$ as our constant. 
$$\begin{align*}
\frac{\partial F}{\partial y}(x,y)&= N(x,y)
\end{align*}$$
---
## Theorem Does Not Hold
If the theorem does not hold, then we must introduce an [[Integration Factor Method]] to solve this. We must introduce a new function, $\mu(x,y)$ which we multiple the entire equation by. 
$$\begin{align*}
\mu(x,y)M(x,y)+\mu(x,y)N(x,y)\frac{dy}{dx}&=  0
\end{align*}$$
We can now write this expression as:
$$\begin{align*}
(\mu M)_y&= (\mu N)_x\\
\implies\mu_yM+\mu M_y&= \mu_xN+\mu N_x
\end{align*}$$
### Finding $\mu$
If we assume that $\mu$ is only a function of $x$, this will give us a property that $\mu_y=0$. This gives us the following:
$$\begin{align*}
0+\mu M_y&= \mu_xN+\mu N_x\\
\implies\frac{\mu_x}{\mu}&= \frac{M_y-N_x}N
\end{align*}$$
This then gives us a first order [[Ordinary Differential Equations|ODE]]. We can then solve this by substituting in the values for $M_y$ and $N_x$, and then solving the first order [[Ordinary Differential Equations|ODE]]. If that fails, we then do the same, assuming $\mu$ is only a function of $y$.
$$\begin{align*}
\mu_yM+\mu M_y&= 0+\mu N_x\\
\implies\frac{\mu_y}{\mu}&= \frac{N_x-M_y}{M}
\end{align*}$$
When we find the correct $\mu$, we can then go forward with the original process, treating $\tilde{M}=\mu M$
and $\tilde{N}=\mu N$ as our $M$ and $N$.