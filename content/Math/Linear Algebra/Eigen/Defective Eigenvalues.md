If the [[Geometric Multiplicity]] of a [[Matrix]] is less than that of the algebraic multiplicity, then this equation has a defective [[Eigenvalues]]. This will  give us an incomplete solution to [[Math/Differential Equations/Differential Equations|Differential Equations]], as we are missing one of the two roots. In order to get this second [[Eigenvalues|Eigenvectors]], we have to solve this equation:
$$
\begin{aligned}
(P-\lambda_1)\vec v_2=\vec v_1
\end{aligned}
$$
>[!Note]
>This is very similar to the [[Characteristic Equation]]

We can then plug this into the form:
$$
\begin{aligned}
\vec x(t)=C_1\vec v_1e^{\lambda _1 t}+C_2(t\vec v_1+\vec v_2)e^{\lambda_1 t}
\end{aligned}
$$