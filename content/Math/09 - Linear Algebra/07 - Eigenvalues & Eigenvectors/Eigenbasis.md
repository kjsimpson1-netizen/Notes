An [[Eigenbasis]] is a [[Basis]] consisting entirely of [[Eigenvector|Eigenvectors]] or [[Eigenfunction|Eigenfunctions]] of a [[Linear Transformation]]. By definition, an eigenbasis is both [[Linear Independence|linearly independent]] and spans the relevant Vector Space or [[Subspace]].

## Vectors

Given enough linearly independent [[Eigenvector|Eigenvectors]], we can form an [[Eigenbasis]] for the vector space on which the [[Matrix]] acts. For example, consider the [[Linear Transformation]] given by:

$$
A=\begin{bmatrix}1&1\\0&2\end{bmatrix}
$$

The corresponding [[Eigenpair|Eigenpairs]] are:

$$
\lambda_1=1,\qquad \vec v_1=\begin{bmatrix}1\\0\end{bmatrix}
$$

$$
\lambda_2=2,\qquad \vec v_2=\begin{bmatrix}1\\1\end{bmatrix}
$$

Since these two [[Eigenvector|Eigenvectors]] are linearly independent, they form an [[Eigenbasis]] for $\mathbb R^2$. We can verify this by forming the change-of-[[Basis]] [[Matrix]]:

$$
P=\begin{bmatrix}|&|\\\vec v_1&\vec v_2\\|&|\end{bmatrix}
=\begin{bmatrix}1&1\\0&1\end{bmatrix}
$$

Since

$$
\det(P)=1\neq0,
$$

$P$ is invertible, meaning that the eigenvectors form a basis. Therefore, any [[Vector]] $\vec v\in\mathbb R^2$ can be expressed as a [[Linear Combination]] of these eigenvectors:

$$
\vec v=\sum_{i=1}^{2}c_i\vec v_i.
$$

More generally, if an $n\times n$ matrix has $n$ linearly independent eigenvectors, then they form an eigenbasis and

$$
\vec v=\sum_{i=1}^{n}c_i\vec v_i.
$$

The coefficients $c_i$ are the coordinates of $\vec v$ in the eigenbasis. In general, they can be found using the inverse of the change-of-basis matrix:

$$
[\vec v]_{\text{eigenbasis}}=P^{-1}[\vec v]_{\text{standard}}.
$$

If the eigenvectors are orthogonal, we can instead find each coefficient independently using the [[Dot Product]]:

$$
c_i=\frac{\vec v_i\cdot\vec v}{\vec v_i\cdot\vec v_i}.
$$

This is effectively a projection of $\vec v$ onto the eigenvector $\vec v_i$. If the eigenvectors are orthonormal, this simplifies to

$$
c_i=\vec v_i\cdot\vec v.
$$

> [!Note] **Projection coefficients**
> The projection formula only works directly when the basis vectors are orthogonal. A general eigenbasis does not necessarily consist of orthogonal eigenvectors, so the coefficients must generally be found using $P^{-1}$.
> If a matrix is defective, it does not have enough linearly independent eigenvectors to form a basis for the entire vector space. In this case, the available eigenvectors span only a proper subspace of the original vector space, and an eigenbasis for the entire space does not exist.

## Functions

The same idea extends to function spaces. Function spaces can be infinite-dimensional. For example, representing an arbitrary sufficiently well-behaved function on an interval generally requires an infinite set of basis functions.
If

$$
\{\phi_1(x),\phi_2(x),\ldots\}
$$

is an [[Eigenbasis]] of eigenfunctions, then a function $f(x)$ in the space can be expressed as

$$
f(x)=\sum_{i=1}^{\infty}c_i\phi_i(x).
$$

The coefficients $c_i$ are the coordinates of $f(x)$ in the eigenfunction basis.
The analogue of the [[Dot Product]] for functions is the [[Function Inner Product]]:

$$
\langle f,g\rangle=\int_a^b f(x)g(x)\,dx.
$$

This can be understood as the continuous analogue of the vector dot product:

$$
\vec u\cdot\vec v=\sum_i u_iv_i.
$$

The discrete sum over vector components becomes an integral over the continuous variable $x$.
If the eigenfunctions are orthogonal under this inner product,

$$
\langle\phi_i,\phi_j\rangle=0\qquad(i\neq j),
$$

then the coefficients can be found using the same projection idea as for orthogonal vectors:

$$
c_i=\frac{\langle\phi_i,f\rangle}{\langle\phi_i,\phi_i\rangle}.
$$

Therefore,

$$
\boxed{c_i=\frac{\displaystyle\int_a^b f(x)\phi_i(x)\,dx}{\displaystyle\int_a^b\phi_i(x)^2\,dx}}
$$

If the eigenfunctions are orthonormal, then

$$
\langle\phi_i,\phi_i\rangle=1,
$$

and the expression simplifies to

$$
\boxed{c_i=\int_a^b f(x)\phi_i(x)\,dx}
$$

If the appropriate [[Function Inner Product]] contains a weight function, then

$$
\langle f,g\rangle_w=\int_a^b w(x)f(x)g(x)\,dx,
$$

and the coefficient becomes

$$
\boxed{c_i=\frac{\displaystyle\int_a^b w(x)f(x)\phi_i(x)\,dx}{\displaystyle\int_a^b w(x)\phi_i(x)^2\,dx}}
$$

The weight function $w(x)$ is the continuous analogue of a weighting matrix in a vector space. In the vector case, a weighted inner product can be written as

$$
\langle\vec u,\vec v\rangle_W=\vec u^{\,T}W\vec v.
$$

Thus, the correspondence is:

$$
\boxed{\vec u\cdot\vec v\quad\longleftrightarrow\quad\int_a^b u(x)v(x)\,dx}
$$

and

$$
\boxed{\vec u^{\,T}W\vec v\quad\longleftrightarrow\quad\int_a^b w(x)u(x)v(x)\,dx}
$$

The overall analogy is therefore:

$$
\boxed{\vec v=\sum_i c_i\vec v_i\quad\longleftrightarrow\quad f(x)=\sum_i c_i\phi_i(x)}
$$

where the $c_i$'s are the coordinates of the vector or function in its respective eigenbasis.
