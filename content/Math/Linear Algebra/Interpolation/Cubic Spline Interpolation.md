This is another form of [[Interpolation]] that takes the form:
$$
$$\begin{aligned}
p_k(t)=a_k(t-t_{k-1})^3+a_k(t-t_{k-1})^3+a_k(t-t_{k-1})^3+d_k,\quad t\in[t_{k-1},t_k]
\end{aligned}$$
$$
Such that $p(t)$ and $p''(t)$ have [[Continuity]].
>[!Note]
>Each polynomial $p_k(t)$ is defined by four coefficients, therefore we required $4N$ unknowns. 

A bonus of using cubic spline is that the [[Condition Number]] does not increase greatly with an increasing number of data points, unlike the [[Vandermonde Matrix]].

## Natural Cubic Spline
A natural cubic spline will set the concavity of the two endpoints of the function to be 0, i.e. $p_1''(t_0)=p_k''(t_N)=0$.
