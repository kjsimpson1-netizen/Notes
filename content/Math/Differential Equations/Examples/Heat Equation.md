This is the equation  for a bar of length $L$ and the change in time for each point along the bar:
$
$
\begin{aligned}
\frac{\partial u}{\partial t}=\alpha ^2\frac{\partial ^2u}{\partial x^2}
\end{aligned}
$
$
>[!Note]
>The the $\frac{\partial ^2u}{\partial x^2}$ represents the [[Diffusion]] term

## Derivation
### One dimension
Letting $u(x,t)$ be the concentration of some quantity, $x$ is space and $t$ is time. If we take a chunk of space such that $x\in(a,b)\quad a,b\in\mathbb{R}$, call it the control volume. Let there also be an internal source/sink, $Q(x,t)$, as well as a flux $J$.  We can derive the heat equation from a conservation law:
$
$
\begin{aligned}
\frac d{dt}\left(\int_a^bu(x,t)dx\right)&= J_\text{in}-J_\text{out}+\int_a^bQ(x,t,u)dx
\end{aligned}
$
$
Then from Fick's law, we have that $J=-D\frac{du}{dx}$. Substituting this in, we have:
$
$
\begin{aligned}
\frac d{dt}\left(\int_a^bu(x,t)dx\right)&= -D\frac{du}{dx}\Big|_{x=a}+D\frac{du}{dx}\Big|_{x=b}+\int_a^bQ(x,t,u)dx\\
\\
\int_a^bu_t(x,t)dx&= \int_a^bDu_{xx}dx+\int_a^bQ(x,t,u)dx
\end{aligned}
$
$
Therefore, for any $a,b$, we must have that:
$$\begin{align}
\boxed{u_t= Du_{xx}+Q(x,t,u)}
\end{align}$$
$
$
\begin{aligned}

\end{aligned}
$
$
