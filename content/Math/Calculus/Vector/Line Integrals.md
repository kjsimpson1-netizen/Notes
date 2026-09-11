---
aliases:
  - Line Integral
---
These are [[Integral|Integrals]] that are taken along a line (shockingly). These are used for taking the work along a curve. 
$$\begin{align*}
\int_C fds=\int_{t=a}^bf\big(x(t),y(t)\big)\big|\vec r\big|dt
\end{align*}$$
Here, $C$ is the line parameterized by $\vec r(t)=\Big\langle x(t),y(t),z(t)\Big\rangle\quad t\in[a,b]$.
>[!Warning]
>The parameterization must only traverse the curve once.

We also have that for a given domain $C$, the following is true:
$$\begin{align*}
\int_{-C}\vec Fd\vec r=-\int_{C}\vec Fd\vec r
\end{align*}$$