These are used to find the solutions to [[Ordinary Differential Equations]] by turning an [[Ordinary Differential Equations]] into an algebraic one. These are a type of [[Transforms]], and will take the form of:
$
$
\begin{aligned}
\mathcal{L}\big\{f(t)\big\}(s)&= \int_0^\infty f(t)e^{-st}dt
\end{aligned}
$
$
After we compute this [[Definite Integral]], we will be given the transformed function,.

| $f(x)$           | $\mathcal{L}\big\{f(t)\big\}(s)$    |
| ---------------- | ----------------------------------- |
| $C$              | $\frac cs, s>0$                     |
| $t^n$            | $\frac{n!}{s^{n+1}},s>0$            |
| $e^{-nt}$        | $\frac1{s+a},s+a>0$                 |
| $\sin(\omega t)$ | $\frac{\omega}{s^2+\omega^2},s+a>0$ |
| $\cos(\omega t)$ | $\frac{s}{s^2+\omega^2},s+a>0$      |
| $u(t-a)$         | $\frac{e^{-as}}s$                   |
| $e^{at}f(t)$     | $F(s+a)$                            |
| $u(t-a)f(t-a)$   | $e^{as}F(s)$                        |

## Existence and Uniqueness
A function $f(t)$ is of exponential order if as $t\to\infty$, we have $\Big|f(t)\Big|<Me^{ct}\qquad M,c\in\mathbb{R}$.
### Existence
$f(t)$ be continuous and of exponential order for a C, then $\mathcal{L}\{f(t)\}(s)$ is defined by all $s>c$.
### Uniqueness
Let $f(t),g(t)$ be continuous and of exponential order. suppose that there exists a constant $C$ such that $\mathcal{L}\{f(t)\}(s)=\mathcal{L}\{g(t)\}(s)$  for $s>c$, then $f(t)=g(t)$ for all $t>0$. 
>[!Note]
>Laplace transforms always have [[Linearity]] due to the properties of integrals
# Solving Equations
In general, in order to solve an [[Ordinary Differential Equations|ODE]] with Laplace transforms, we just take the Laplace transform of both sides of the equation, and then rearrange this, solving for the $\mathcal{L}$ term and then taking the inverse Laplace transform:
$
$
\begin{aligned}
\mathcal L(ax^2+bx+c)=\mathcal L(f(x))
\end{aligned}
$
$
