---
aliases:
  - Eigenvectors
---
An eigenvector is defined to be the [[vector]] for which when it is multiplied by a [[Matrix]], it will return a scaled version of that [[Vector]], which is scaled by it's corresponding [[Eigenvalues|Eigenvalue]]. It is given by this equation:
$$
\begin{aligned}
A\vec v&= \lambda \vec v
\end{aligned}
$$
## Finding the Eigenvector
In order to find the numerical values for [[Eigenvector|Eigenvectors]], we must first find the [[Eigenvalues|Eigenvalue]]. Once we have solve for the [[Eigenvalues]], we can once again use:
$$
\begin{aligned}
(A-\lambda\mathbb{I})\vec v=0
\end{aligned}
$$
To solve for the eigenvectors. We can plug in the corresponding [[Eigenvalues]] and solve the [[Linear System]]to get the [[Eigen Pairs]].