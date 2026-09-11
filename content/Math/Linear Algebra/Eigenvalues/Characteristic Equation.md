This is the equation to calculate the [[Eigenvalues]] of a [[Matrix]], and in order to calculate [[Eigenvalues|Eigenvectors]], we must find where the following is true:
$$
$$\begin{aligned}
\det(A-\lambda I)&= 0
\end{aligned}$$
$$
For an $n\times n$ [[Linear Transformation]] [[Matrix]], there will be $n$ different values.
## $2\times 2$ Matrix
For a two by two matrix, we can express the characteristic equation as:
$$
$$\begin{aligned}
\lambda ^2-\text{Tr}(A)\lambda+\det(A)&= 0
\end{aligned}$$
$$
Where the square of the [[Eigenvalues]] is equal to the [[Trace]] and the [[Determinant]]
>[!Note]
>The [[Trace]] is equal to the sum of the [[Eigenvalues]] and the [[Determinant]] is equal to the product of the [[Eigenvalues]]

## $3\times3$ Matrix
For a three by three [[Matrix]], we are given the following formula:
$$
$$\begin{aligned}
\lambda^3-\text{Tr}(A)\lambda ^2+c_2\lambda-\det(A)&= 0
\end{aligned}$$
$$
The equation for $c_2$ is the product of all the unique combinations of the diagonal minus the unique combinations of the other diagonals. However, we can also just use the characteristic equation. 
