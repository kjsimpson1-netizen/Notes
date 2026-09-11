---
aliases:
  - Kernel
---
A nullspace of a [[Matrix]], also known as the kernel, is a set of vectors that are mapped to 0 by $(A-\lambda I)\vec v$. If there exists an [[Inverse Matrices]] of $A$, then the only vector that applies is 0. However, if it is non-invertible, then there are multiple values. This is the same as finding a non-trivial [[Linear Relation]] of the columns of $A$. The formal definition of a nullspace is:
$
\begin{aligned}
N(A)=\set{\vec x\in \mathbb R^n:A\vec x=\vec 0}
\end{aligned}
$
>[!Theorems]
>1. If $A$ is a $m\times n$ [[Matrix]], then the nullspace is a [[Subspace]] of $\mathbb R^n$
>2. $A$ has the [[LU Decomposition]] of $A=LU$, then $N(L)=N(U)$

