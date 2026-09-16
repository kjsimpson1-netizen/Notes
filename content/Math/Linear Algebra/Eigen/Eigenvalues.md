---
aliases:
  - Eigenvalue
---
An eigenvalue, $\lambda$, is defined to be the amount of scaling that is applied an [[Eigenvector]] when a [[matrix]] is multiplied by one it's [[Eigenvector]]:
$$
\begin{aligned}
&\qquad A\vec v= \lambda \vec v\\
\hline\\
A&= \text{Transformation Matrix}\\
\vec v&= \text{Eigenvector}\\
\lambda&= \text{Eigenvalue}
\end{aligned}
$$
We can find the [[Eigenvalues]] using the [[Characteristic Equation]].
## Finding the Eigenvalue
In order to find the numerical values for [[Eigenvalues|Eigenvalues]], we can take the definition above and rework it:
$$
\begin{aligned}
(A-\lambda\mathbb{I})\vec v&= 0
\end{aligned}
$$
And in order for this to be true for the non trivial case of $\vec v=\vec 0$, we can solve for:
$$
\begin{aligned}
A-\lambda\mathbb{I}&= 0
\end{aligned}
$$
For a $2\times2$ [[Matrix]], this will give us the [[Characteristic Equation]], and the roots of this equation will give us the [[Eigenvalues|Eigenvalue]]. For and $n\times n$ [[Matrix]], it will have $n$ eigenvalues (except in certain cases with repeated eigenvalues, and these eigenvalues are considered [[Defective Eigenvalues]]).