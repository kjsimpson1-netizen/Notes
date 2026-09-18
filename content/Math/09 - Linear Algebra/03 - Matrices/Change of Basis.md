A change of basis allows us to express the same state or [[vector]] using a different [[basis]]. Suppose we have two orthonormal bases ${\ket{e_i}}$ and ${\ket{f_i}}$.
## Resolution of the Identity
For an orthonormal basis ${\ket{e_i}}$, the sum
$$
\sum_i\ket{e_i}\bra{e_i}=\hat I
$$
is the resolution of the [[Identity Matrix]]. Therefore, for any state $\ket{\Psi}$,
$$
\sum_i\Big(\ket{e_i}\bra{e_i}\Big)\ket{\Psi}=\ket{\Psi}.
$$
Rearranging gives
$$
\ket{\Psi}=\sum_i\ket{e_i}\braket{e_i|\Psi}.
$$
The quantity
$$
\braket{e_i|\Psi}
$$
is the coefficient of $\ket{\Psi}$ in the basis ${\ket{e_i}}$. Thus, the state can be written as
$$
\ket{\Psi}=\sum_i c_i\ket{e_i}, \qquad c_i=\braket{e_i|\Psi}.
$$
## Change of Basis
Suppose we want to express a state in the ${\ket{e_i}}$ basis instead of the ${\ket{f_i}}$ basis. We can insert the resolution of the identity in the $e$ basis:
$$
\ket{\Psi}=\sum_i\ket{e_i}\braket{e_i|\Psi}.
$$
Similarly, each vector in the $f$ basis can be expressed using the $e$ basis:
$$
\ket{f_j}=\sum_i\ket{e_i}\braket{e_i|f_j}.
$$
The coefficients
$$
\braket{e_i|f_j}
$$
describe how the $f$ basis vectors are represented in the $e$ basis. These coefficients form the change-of-basis matrix:
$$
\boxed{O_{f\to e}=\left[\braket{e_i|f_j}\right]}
$$
Explicitly,
$$
\boxed{ O_{f\to e} = \begin{pmatrix} \braket{e_1|f_1} & \braket{e_1|f_2} & \cdots \\ \braket{e_2|f_1} & \braket{e_2|f_2} & \cdots \\ \vdots & \vdots & \ddots \end{pmatrix} }
$$
If a state has coordinates $[\Psi]_f$ in the $f$ basis, then its coordinates in the $e$ basis are
$$
\boxed{[\Psi]_e=O_{f\to e}[\Psi]_f}.
$$
For orthonormal bases, the inverse transformation is given by the [[Adjoint]]:
$$
\boxed{O_{e\to f}=O_{f\to e}^\dagger}.
$$
Therefore,
$$
[\Psi]_f=O_{f\to e}^\dagger[\Psi]_e.
$$
## Key Idea
The resolution of the identity allows us to expand a state in a particular basis, while the change-of-basis matrix converts the coordinates of that state from one basis to another. The physical state $\ket{\Psi}$ remains the same; only its representation changes.