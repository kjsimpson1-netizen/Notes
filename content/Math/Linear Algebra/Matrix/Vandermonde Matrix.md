This is the matrix that allows us to find the [[Polynomial Interpolation]] of a data set. The Vandermonde [[matrix]] is given by:
$$\begin{align*}
A=\begin{bmatrix}
1&t_0&\cdots&t_0^d\\
1&t_1&\cdots&t_0^1\\
\vdots&\vdots&\ddots&\vdots\\
1&t_d&\cdots &t_d^d
\end{bmatrix}
\end{align*}$$
From this, we have that the [[Determinant]] of the Vandermonde matrix as:
$$\begin{align*}
\det(A)=\prod_{0\le i\le j\le d}(t_j-t_i)
\end{align*}$$
