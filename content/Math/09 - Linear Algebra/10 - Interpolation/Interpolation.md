Interpolation is the process of constructing a function, called an **interpolant**, that matches a given set of data points and approximates the underlying true function.
There are infinitely many possible functions that can pass through a given set of data points. Therefore, additional constraints are needed to determine a particular interpolation strategy.
## Global Interpolation
Consider an interval
$$
x\in[a,b]
$$
divided into $N$ subintervals, each with width
$$
h=\frac{b-a}{N}.
$$
On each subinterval, the function can be approximated using a polynomial. Combining these local approximations gives a global approximation $F_N(x)$ of the true function $f(x)$.
## Convergence
An interpolation strategy **converges** if the approximation approaches the true function as the number of subdivisions increases:
$$
\lim_{N\to\infty}\left\|F_N(x)-f(x)\right\|_\infty=0.
$$
## Order of Convergence
If there exists a constant $C>0$ such that
$$
\left\|F_N(x)-f(x)\right\|_\infty\le Ch^p,
\qquad p>0,
$$
then the interpolation method is said to have **order of convergence $p$**.
The exponent $p$ determines how quickly the error decreases as the mesh width $h$ decreases.
* $p=1$: first-order convergence
* $p=2$: second-order convergence
* $p=3$: third-order convergence
