The error in an [[10 - Interpolation|Interpolation]] on an [[Interval]] $x\in[a,b]$ is defined to be:$$
\begin{aligned}
e(x)=f(x)-I(x)
\end{aligned}
$$Where $I(x)$ is the interpolant of the function $f(x)$. 
## Error and Auxiliary Functions
In order to evaluate the error, we need to introduce an auxiliary function in terms of a dummy variable $y$:$$
\begin{aligned}
g(y)=e(y)-w(y)K(x)
\end{aligned}
$$
Here, $w(y)$ is the [[node polynomial]] is built from [[10 - Interpolation|Interpolation]] conditions, and $K(x)$ is a constant chosen so that our auxiliary function $g(y=x)=0$:
$$
\begin{aligned}
K(x)&= \frac{e(y)}{w(y)}
\end{aligned}
$$
## Zeroes of $g(y)$
Since by the interpolation conditions, we have that $I(x_0)=f(x_0)$ and therefore $e(x_0)=0$. Since $g(x)$ is built by the same conditions, we also have $g(x_0)=0$. This means that is $f(x)$ has at least $N$ zeroes on $x\in[a,b]$, then $g(x)$ must also have $N$ zeroes. However, by introducing $y$ as a new variable, we can force $g(x=y)=0$, thus $g(x)$ has $N+1$ zeroes. We can now apply [[Rolle's Theorem]] to get:
$$
\begin{aligned}
g^{(m)}(\zeta)=0\quad,\zeta\in[a,b]
\end{aligned}
$$
## Differentiating
We can now take $m$ derivatives of $g(x)$ to get:
$$
\begin{aligned}
g^{(m)}(y)&= e^{(m)}(y)-w^{(m)}(y)K(x)\\
&= f^{(m)}(y)-I^{(m)}(y)-w^{(m)}(y)K(x)
\end{aligned}
$$Since we have that $g^{(m)}(\zeta)=I^{(m)}(\zeta)=0$, and $w^{(m)}(\zeta)=m!$thus:$$
\begin{aligned}
K(x)&= \frac{f^{(m)}(\zeta)}{m!}
\end{aligned}
$$We can then substitute $K(x)$ in:
$$
\begin{aligned}
e(y)=w(y)\left(\frac{f^{(m)}(\zeta)}{m!}\right)
\end{aligned}
$$
