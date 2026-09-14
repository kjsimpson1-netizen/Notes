If we want to raise a [[Matrix]] to a power, we can easily do this if the vector that it's being multiplied by is one of it's [[Eigenvalues|Eigenvectors]]. $$\begin{align*}
A^k\vec v&= \lambda^k \vec v
\end{align*}$$
This can then be solved by expressing $\vec v$ as a [[Linear Combinations]] of the [[Eigenvalues|Eigenvectors]], with the [[Eigenvalues]] raised to the $kth$ power. 
$$\begin{align*}
A^k\vec v&= A^k(c_1\vec v_1+c_2\vec v_2+c_3\vec v_3+...+c_n\vec v_n)\\
&= c_1A^k\vec v_1+c_2A^k\vec v...
\end{align*}$$
We can then replace $A$ with the corresponding eigenvalues:
$$\begin{align*}
A^k\vec v&= c_1\lambda_1\vec v_1+c_2\lambda_2\vec v_2...
\end{align*}$$From this point, we can expand and simplify as necessary. 
>[!Note]
>It is important that the eigenvector $\vec v\neq0$, and that the equality above holds.
