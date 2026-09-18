The error when approximating a function using a [[Taylor Polynomials|Taylor Polynomial]] can be expressed in terms of a higher derivative of the function evaluated at some intermediate point.
## Error Theorem
For a Taylor polynomial of degree $n$ about $x=a$, the error is
$$
e_n(x)=f(x)-P_n(x)=\frac{f^{(n+1)}(\zeta)}{(n+1)!}(x-a)^{n+1}
$$
for some $\zeta$ between $a$ and $x$.
Therefore,
$$
\boxed{e_n(x)=\frac{f^{(n+1)}(\zeta)}{(n+1)!}(x-a)^{n+1}}
$$
## Error Bound
If
$$
\left|f^{(n+1)}(x)\right|\le K_{n+1}
$$
over the relevant interval, then
$$
|e_n(x)|\le\frac{K_{n+1}}{(n+1)!}|x-a|^{n+1}
$$
This provides an upper bound on the approximation error.
## Connection to Interpolation
The Taylor polynomial error has a similar structure to interpolation error. In both cases, the error depends on:
* A higher derivative of $f$
* A factorial term
* A power of the distance between points
The derivation of these error formulas relies on [[Rolle's Theorem]].