In order to find the steady state of a [[Neumann Boundary Conditions]] [[Partial Differential Equations]], we can solve by first integrating over the differential equation:
$$
\begin{aligned}
\int_0^Lu_tdx&= \int_0^LDu_{xx}dx
\end{aligned}
$$
We can then pull out the complete time derivative to get:
$$
\begin{aligned}
\frac d{dt}\int_0^Ludx&= D\Big|_{x=0}^{x=L}=0
\end{aligned}
$$
Therefore, $\frac d{dt}\int_0^Ldx=0$. We can then integrate over $dt$ to find:
$$
\begin{aligned}
\int_0^Ludx&= u_S
\end{aligned}
$$
We can then evaluate as $t\to\infty$ and 

