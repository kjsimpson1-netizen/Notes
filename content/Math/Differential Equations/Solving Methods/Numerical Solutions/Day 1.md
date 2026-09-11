## Floating Point Approximation
On computers, when looking for exact values, there is always a floating point approximation. This means for a given value of $x\in\mathbb{R}$, the value given is $x(1+c\epsilon),\epsilon\in\mathbb{R}$, where $|\epsilon|<10^{-16}$ and $|c|\lt1$. In order to get this as close as possible, we want the relative error to be as small as possible. 
### Vectors
Let there be a vector $\vec u$ such that:
$$
$$
\begin{aligned}
\vec u&= \begin{bmatrix}
u_1&u_2&u_3&\dots&u_n
\end{bmatrix}
\end{aligned}
$$
$$
For this vector, there are a variety of norms that we can take:
- [[Norm|Euclidian Norm]]
- [[Maximum Norm]]
- [[One Norm]]
- [[Matrix Norm]]
---
Say that we have an invertible matrix $A$, such that $A\vec x=\vec b$. If we want to find $\vec x$, we can express this as $\vec u=A^{-1}\vec b$. This describes [[Gaussian Elimination]] back substitution. However, when done using computational tools, there will be floating point errors in $\vec u,\vec b,\text{ and }A$ that will propagate throughout the solution. 
$$
$$
\begin{aligned}
(A+\epsilon E)(\vec u+\epsilon y)&= \vec b+\epsilon d
\end{aligned}
$$
$$
We can say that $|E_{ij}|<|A_{ij}|$ which implies that $||E_{ij}||_\infty\le ||A||_\infty$. We also have that $|d_j|\le |b_j|$, and this implies that $||\vec d||_\infty\le||\vec b||_\infty\le||A||_\infty||\vec x||_\infty$. For this, we will neglect all errors on the scale of $\epsilon^2$. This gives us that the order $\epsilon$ terms leave:
$$
$$
\begin{aligned}
A\vec y&= -E\vec x+\vec d
\end{aligned}
$$
$$
From this we have:
$$
$$
\begin{aligned}
\vec y&\approx -A^{-1}E\vec x+A^{-1}\vec d
\end{aligned}
$$
$$
From this, we can say the following about the magnitude of the errors:
$$
$$
\begin{aligned}
||\vec y||_\infty&\le ||A^{-1}||_\infty||A||_\infty||\vec x||_\infty+||A^{-1}||_\infty||A||_\infty||\vec x||_\infty\\
&\le 2\underbrace{||A^{-1}||_\infty||A||_\infty}_\text{Condition Number}||\vec x||_\infty
\end{aligned}
$$
$$
The [[Condition Number]] describes the magnitude of the error that the matrix will give. 