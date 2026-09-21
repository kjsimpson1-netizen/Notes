---
aliases:
  - LTI System
---
LTI [[System|Systems]] are very nice to work with, and they can be defined as so if the following two conditions hold:
## Linear System
A [[System]] is defined to be linear if holds under both additivity and homogeneity (scaling). More formally expressed, a [[System]] is linear if the following holds:
$$
\begin{aligned}
L\{ax(t)+by(t)\}\to aL\{x(t)\}+bL\{y(t)\}
\end{aligned}
$$
## Time Invariant System
These are systems that hold the same properties, regardless of when they are observed. Put formally:$$
\begin{aligned}
x(t-t_0)&= y(t-t_0)\quad\forall t_0\in\mathbb{R}\\
x[n-n_0]&= y[n-n_0]\quad\forall n_0\in\mathbb{R}
\end{aligned}
$$
