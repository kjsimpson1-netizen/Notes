For a scalar-valued function $f(\vec{x})$, where $\vec{x}\in\mathbb{R}^N$, [[Non-Linear Optimization]] seeks to find the values of $\vec{x}$ that minimize or maximize $f(\vec{x})$.

### Finding Extrema

At an extremum $\vec{x}_*$, the gradient must be zero:

$$
\nabla f(\vec{x}_*)=0
$$

Therefore, finding the extrema of $f$ can be treated as a root-finding problem for the gradient $\nabla f(\vec{x})$.

The [[Hessian Matrix]] can then be used to determine the nature of a stationary point. The Hessian is the matrix of second partial derivatives:

$$
H(\vec{x})=
\nabla^2f(\vec{x})
$$

At a stationary point $\vec{x}_*$:

* If $H(\vec{x}**)$ is **positive definite**, $\vec{x}**$ is a local minimum.
* If $H(\vec{x}**)$ is **negative definite**, $\vec{x}**$ is a local maximum.
* If $H(\vec{x}**)$ is **indefinite**, $\vec{x}**$ is a saddle point.

### Gradient Descent

For large-scale problems, directly solving $\nabla f(\vec{x})=0$ or working with the [[Hessian Matrix]] can become computationally expensive. An alternative is **gradient descent**, which iteratively moves $\vec{x}$ in the direction of steepest decrease of $f$.

The update rule is:

$$
\vec{x}_{n+1}
=
\vec{x}_n
-
\lambda\nabla f(\vec{x}_n)
$$

where $\lambda$ is the **learning rate** (or step size).

The gradient $\nabla f(\vec{x}_n)$ points in the direction of greatest increase of $f$. Therefore, subtracting the gradient moves $\vec{x}_n$ in the direction of greatest decrease.

The learning rate $\lambda$ determines the size of each step:

* A **small** $\lambda$ produces slow convergence.
* A **large** $\lambda$ can cause the method to overshoot the minimum or become unstable.
* An appropriate $\lambda$ allows the algorithm to converge efficiently.

The learning rate is a **computational parameter** rather than a property of the function itself. Its value must be chosen to produce effective convergence for the particular problem.

Gradient descent is primarily suited to finding **local minima**. For a sufficiently smooth function, the method continues updating $\vec{x}$ until the gradient becomes sufficiently small:

$$
||\nabla f(\vec{x}_n)||\approx 0
$$

At this point, $\vec{x}_n$ is taken as an approximation to a stationary point.


