Very similar to how the [[Tangent Line]] is the line that is parallel and just barely touches the function at the evaluated point, the tangent plane is the one that barely touches the surface and is completely parallel (or more accurately, parallel to the [[Normal Line]]. Instead of using regular [[Derivative|Derivatives]] like we did for the [[Tangent Line]], we will now use [[Partial Derivatives]]. 
### $z=f(x,y)$
For questions of this form, we can solve by following the following steps:
1. The normal vector will be the defined by:$$
$$
\begin{aligned}
\vec v_\perp&= \begin{bmatrix}
-f_x(x_0,y_0)\\
-f_y(x_0,y_0)\\
f(x_0,y_0)
\end{bmatrix}
\end{aligned}
$$
$$
2. This can be rewrote in [[Parametric Formula]] by:$$
$$
\begin{aligned}
\vec x&= P_0+t \begin{bmatrix}
-f_x(x_0,y_0)\\
-f_y(x_0,y_0)\\
1
\end{bmatrix}
\end{aligned}
$$
$$
### $f(x,y,z)= C\qquad C\in\mathbb{R}$
We can find the tangent plane to these forms of equations by doing the following (assuming that all components of the [[Gradient]] at $P_0$ are non-zero):
#### [[Point-Normal Formula]]
The following is true, where $P_0=x_0,y_0,z_0$:
$$
$$
\begin{aligned}
\nabla f(P_0)\cdot(\vec x-P_0)=0
\end{aligned}
$$
$$
#### [[Parametric Formula]]:
$$
$$
\begin{aligned}
\vec x&= P_0+t\nabla f(P_0)
\end{aligned}
$$
$$

