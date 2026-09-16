The [Condition Number](Condition Number) describes how sensitive the final solution of a problem is to small perturbations in the initial conditions. For a [Matrix](Matrix) $A$, this is denoted by $\text{cond}(A)$ and is given by:

$$
\text{cond}(A) = ||A||\,||A^{-1}||
$$

We can also interpret the condition number as the ratio of the largest change to the smallest change produced by $A$ when acting on a [unit vector](unit vector):

$$
\text{cond}(A) = \frac{\text{Largest Change}}{\text{Smallest Change}}
$$

Therefore,

$$
\text{cond}(A)\in[1,\infty)
$$

A condition number close to $1$ indicates that the matrix is relatively insensitive to perturbations, while a large condition number indicates that small errors can be significantly amplified.

### Error Propagation

Consider a linear system

$$
A\vec{x}=\vec{b}
$$

where we want to find

$$
\vec{x}=A^{-1}\vec{b}
$$

When this is solved computationally, floating-point errors introduce small perturbations to $A$ and $\vec{b}$. We can represent these perturbations as

$$
(A+\epsilon E)(\vec{x}+\epsilon\vec{y}) = \vec{b}+\epsilon\vec{d}
$$

where $E$ and $\vec{d}$ represent the errors in $A$ and $\vec{b}$, respectively, and $\epsilon$ represents the scale of the perturbation.

Neglecting terms of order $\epsilon^2$, we obtain

$$
A\vec{y}=-E\vec{x}+\vec{d}
$$

Multiplying by $A^{-1}$ gives

$$
\vec{y}=-A^{-1}E\vec{x}+A^{-1}\vec{d}
$$

Thus, the error in the solution depends on $A^{-1}$. Using the infinity norm, we can bound the magnitude of the error:

$$
||\vec{y}||_\infty
\leq
||A^{-1}||_\infty
||E||_\infty
||\vec{x}||_\infty
+
||A^{-1}||_\infty
||\vec{d}||_\infty
$$

If the perturbations satisfy

$$
||E||_\infty\leq||A||_\infty
$$

and

$$
||\vec{d}||_\infty
\leq
||\vec{b}||_\infty
\leq
||A||_\infty||\vec{x}||_\infty
$$

then

$$
||\vec{y}||_\infty
\leq
2||A^{-1}||_\infty||A||_\infty||\vec{x}||_\infty
$$

Since

$$
\text{cond}(A)=||A^{-1}||_\infty||A||_\infty
$$

we can write

$$
||\vec{y}||_\infty
\leq
2\,\text{cond}(A)||\vec{x}||_\infty
$$

This demonstrates why the condition number is important in numerical computation: **it determines how strongly small perturbations and floating-point errors can be amplified in the final solution.** A poorly conditioned matrix can therefore produce a large error in $\vec{x}$ even when the errors in $A$ and $\vec{b}$ are very small.
