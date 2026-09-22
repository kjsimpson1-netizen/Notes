The [[Spectral Theorem]] states that any [[Hermitian Matrix]] has **real [[Eigenvalues]]** and can be [[Diagonalization|diagonalized]] using an orthonormal basis of [[Eigenvector|eigenvectors]].

In particular, a Hermitian matrix can be written as
$$A=U\Lambda U^\dagger,$$
where $\Lambda$ is a diagonal matrix containing the eigenvalues of $A$, and $U$ is a unitary matrix whose columns are the corresponding eigenvectors.

An equivalent form is the **spectral decomposition**, where an [[Operator]] $\hat O$ can be expressed in terms of its [[Eigenbasis]]:
$$\boxed{\hat O=\sum_i \lambda_i\ket{\lambda_i}\bra{\lambda_i}}$$
where $\lambda_i$ are the [[Eigenvalues]] and $\ket{\lambda_i}$ are the corresponding orthonormal [[Eigenvector|eigenvectors]].

The operator
$$\ket{\lambda_i}\bra{\lambda_i}$$
is the [[Projector]] onto the eigenspace associated with $\lambda_i$.

> [!NOTE]
> Hermitian $\neq$ positive. A Hermitian matrix can have positive, negative, or zero eigenvalues. If all eigenvalues satisfy $\lambda_i\geq0$, the matrix is **positive semidefinite**.