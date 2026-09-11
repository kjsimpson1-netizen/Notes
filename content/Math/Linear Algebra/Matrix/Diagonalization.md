When a matrix has been put into diagonal form, this is called diagonalizing the matrix. This is useful when we are trying to calculate a [[Matrix]] raised to a $kth$ power. We can do this by:
$$
$$
\begin{aligned}
A&= (TDT^{-1})^k=\begin{bmatrix}
\vec v_1&\vec v_2&\vec v_3...\vec v_n
\end{bmatrix}\begin{bmatrix}
    \lambda_1^k & 0 & 0 & \cdots & 0 \\
    0 & \lambda_2^k & 0 & \cdots & 0 \\
    0 & 0 & \lambda_3^k & \cdots & 0 \\
    \vdots & \vdots & \vdots & \ddots & \vdots \\
    0 & 0 & 0 & \cdots & \lambda_n^k
\end{bmatrix}\begin{bmatrix}
\vec v_1&\vec v_2&\vec v_3...\vec v_n
\end{bmatrix}^{-1}
\end{aligned}
$$
$$
Where the matrix $D$ is the [[Identity Matrix]] of the nth [[Eigenvalues]] raised to the kth power and the [[Matrix]] $T$ is a [[Matrix]] of columns of the [[Eigenvalues|Eigenvectors]]. 