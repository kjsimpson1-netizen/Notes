The **Bisection Method** is a numerical method for finding a root of a function. It is relatively general because it only requires the function $f(x)$ to be [[Continuity|Continuous]] over an interval $[a,b]$.

If

$$
\text{sgn}(f(a))\neq\text{sgn}(f(b))
$$

then, by the [[Intermediate Value Theorem]], there must exist some $x_*\in(a,b)$ such that

$$
f(x_*)=0.
$$

### Algorithm

We begin by evaluating the midpoint of the interval:

$$
x_1=\frac{a+b}{2}
$$

We then evaluate $f(x_1)$ and determine which half of the interval contains the root.

* If $\text{sgn}(f(x_1))\neq\text{sgn}(f(a))$, then the root lies in $[a,x_1]$.
* If $\text{sgn}(f(x_1))=\text{sgn}(f(a))$, then the root lies in $[x_1,b]$.

The interval is therefore reduced by half after each iteration. We then repeat the process using the new interval and its midpoint.

For example, if the root is determined to lie in $[a,x_1]$, the next midpoint is

$$
x_2=\frac{a+x_1}{2}.
$$

If instead the root lies in $[x_1,b]$, then

$$
x_2=\frac{x_1+b}{2}.
$$

This process is repeated until the interval, or equivalently the error in the approximation, is sufficiently small.

### Convergence

Let $B_n$ represent the error or interval bound after $n$ iterations. Since the interval is halved at every iteration,

$$
B_{n+1}=\frac{1}{2}B_n.
$$

More generally, the convergence of a numerical method can be described by

$$
B_{n+1}\approx C B_n^p
$$

where $C$ is the **convergence factor** and $p$ is the **order of convergence**.

For the Bisection Method,

$$
C=\frac{1}{2}
$$

and

$$
p=1.
$$

Thus, Bisection has **linear convergence**. The error decreases by approximately a factor of $2$ with every iteration.

The Bisection Method is therefore guaranteed to converge when $f$ is continuous on $[a,b]$ and $f(a)$ and $f(b)$ have opposite signs. However, its linear convergence makes it slower than methods such as [[Newton-Raphson Method]] when those methods can be applied successfully.


