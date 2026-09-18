**Linear interpolation** approximates a function using straight-line segments between neighboring data points. For an interval divided into $N$ subintervals, linear interpolation uses the $N+1$ function values at the subinterval endpoints. On each subinterval, the interpolant is equivalent to a [[Secant Lines]] approximation.
## Local Linear Approximation
On a subinterval centered at $x_j$, a linear approximation can be written as
$$
f(x)\approx f(x_j)+f'(x_j)(x-x_j).
$$
The interpolation error is
$$
f(x)-L(x)=\frac{f''(\zeta)}{2}(x-x_j)^2,
$$
for some
$$
\zeta\in\left(x_j-\frac h2,x_j+\frac h2\right).
$$
Define
$$
K_n:=\max_{x\in[a,b]}\left|f^{(n)}(x)\right|.
$$
Then
$$
|f(x)-L(x)|\le K_2\frac{h^2}{8}.
$$
This shows that the local linear approximation has an error proportional to $h^2$.
## Reference Coordinate
Consider a subinterval $[x_{i-1},x_i]$ with width
$$
h=x_i-x_{i-1}.
$$
Introduce the reference coordinate
$$
y=\frac{x-x_{i-1}}{h}.
$$
Thus,
$$
x=x_{i-1}+hy.
$$
At the endpoints,
$$
x=x_{i-1}\implies y=0
$$
and
$$
x=x_i\implies y=1.
$$
## Shape Functions
The linear interpolant can be written as
$$
I(y)=f_{i-1}(1-y)+f_i y.
$$
The functions $1-y$ and $y$ are called **reference shape functions**.
They satisfy the interpolation conditions
$$
I(0)=f_{i-1},
\qquad
I(1)=f_i.
$$
Thus, $I(y)$ is the straight line connecting the two endpoint values.
## Interpolation Error
The error in the linear interpolant is
$$
f(y)-I(y)=\frac12y(y-1)\frac{d^2f}{dy^2}(\zeta),
$$
for some $\zeta\in(0,1)$.
Since
$$
\max_{0\le y\le1}|y(y-1)|=\frac14,
$$
we obtain the corresponding error bound. In terms of the physical coordinate $x$, the global interpolation error satisfies
$$
\left\|f-F_N\right\|_\infty\le K_2\frac{h^2}{8},
$$
where
$$
K_2=\max_{x\in[a,b]}|f''(x)|.
$$
Therefore, linear interpolation has **second-order convergence**:
$$
\left\|f-F_N\right\|_\infty=O(h^2).
$$
## Global Approximation
Applying linear interpolation on every subinterval produces a global piecewise-linear approximation $F_N(x)$ of $f(x)$.
Although each individual approximation is only linear, the overall approximation converges to the true function as $h\to0$:
$$
\lim_{N\to\infty}\left\|F_N-f\right\|_\infty=0.
$$
## Limitation
A piecewise linear approximation generally has discontinui