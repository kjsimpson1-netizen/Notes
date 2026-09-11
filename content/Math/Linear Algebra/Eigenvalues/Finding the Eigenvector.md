If we are given a [[Eigenvalues]] and the corresponding [[Matrix]], we can find the eigenvector by doing the following:
$
$
\begin{aligned}
(A-\lambda I)\vec v&= 0
\end{aligned}
$
$
From this we can take the term in brackets and solve the [[Homogeneity|Homogenous]] solution by solving the [[Linear System]].
## Null Space
Instead of using the [[Characteristic Equation]], we can use the [[Nullspace]], or the [[Nullspace|Kernel]], to find it instead. Because $(A-\lambda I)\vec v=0$, and $\vec v\neq0$, then the term $A-\lambda I$ must equal zero. Therefore, the [[Eigenvalues|Eigenvectors]] of the [[Matrix]] is equivalent to:
$
$
\begin{aligned}
\ker(A-\lambda I)
\end{aligned}
$
$
However, in order for this to work, the columns of $A$ must have [[Linear Independence]]. 
>[!Note]
>If we do it this way, and we see that the jth row of the [[Matrix]] is equal to $\alpha \vec e_j$, then we can say that the eigen pair is $\{\alpha,\vec e_j\}$.

