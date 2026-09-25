The error in an [[10 - Interpolation|Interpolation]] on an [[Interval]] $x\in[a,b]$ is defined to be:
$$e(x)=f(x)-I(x)$$
Where $I(x)$ is the interpolant of the function $f(x)$. 
## Error and Auxiliary Functions
In order to evaluate the error, we need to introduce an auxiliary function in terms of a dummy variable $y$:
$$g(y)=e(y)-w(y)K(x)$$
Here, $w(y)$ is the [[node polynomial]] built from [[10 - Interpolation|Interpolation]] conditions, and $K(x)$ is a constant chosen so that our auxiliary function $g(x)=0$:
$$K(x)=\frac{e(x)}{w(x)}$$
## Zeroes of $g(y)$
Since by the interpolation conditions, we have $I(x_i)=f(x_i)$ for all $m$ nodes $x_i$, we have $e(x_i)=0$ and $g(x_i)=0$. This means $g(y)$ has at least $m$ zeroes corresponding to the interpolation nodes on $x\in[a,b]$. By forcing $g(x)=0$ at our evaluation point $x$, $g(y)$ has $m+1$ distinct zeroes. We can now apply [[Rolle's Theorem]] repeatedly to get:
$$g^{(m)}(\zeta)=0\quad,\zeta\in[a,b]$$
## Differentiating
We can now take $m$ derivatives of $g(y)$ with respect to $y$ to get:
$$g^{(m)}(y)= e^{(m)}(y)-w^{(m)}(y)K(x) = f^{(m)}(y)-I^{(m)}(y)-w^{(m)}(y)K(x)$$
Since we have that $g^{(m)}(\zeta)=0$, $I^{(m)}(\zeta)=0$ (since $I$ is a polynomial of degree at most $m-1$), and $w^{(m)}(\zeta)=m!$, thus:
$$K(x)=\frac{f^{(m)}(\zeta)}{m!}$$
We can then substitute $K(x)$ back into $e(x) = w(x)K(x)$:
$$e(x)=w(x)\left(\frac{f^{(m)}(\zeta)}{m!}\right)$$