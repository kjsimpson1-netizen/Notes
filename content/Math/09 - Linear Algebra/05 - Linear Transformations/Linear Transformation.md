A **linear transformation** is a function between vector spaces that preserves Vector Addition and Scalar Multiplication.

A linear transformation takes an input [[Vector]] and produces exactly one output vector.

$$
T:\mathbb{R}^n\rightarrow\mathbb{R}^m
$$

The input vector belongs to the **domain**, and the output belongs to the **codomain**.

> [!Note]
> The **domain** is the set of possible inputs.
>
> The **codomain** is the set where the outputs live.
>
> The **image** is the set of outputs that are actually produced by the transformation.

## Goal of a Linear Transformation

A linear transformation can be represented using a [[Matrix]]:

$$
T(\vec{x})=M_T\vec{x}
$$

where:

* $T$ is the linear transformation
* $M_T$ is the **transformation matrix**
* $\vec{x}$ is the input vector

## Representation of $\vec{x}$

Any vector $\vec{x}$ can be expressed as a [[Linear Combination]] of the standard basis vectors:
$$
\vec{x}
=
\begin{bmatrix}
x_1\\
x_2\\
\vdots\\
x_n
\end{bmatrix}
=
x_1\vec e_1+x_2\vec e_2+\cdots+x_n\vec e_n
$$
where

$$
\vec e_1=
\begin{bmatrix}
1\\
0\\
\vdots\\
0
\end{bmatrix},
\qquad
\vec e_2=
\begin{bmatrix}
0\\
1\\
\vdots\\
0
\end{bmatrix},
\qquad
\ldots,
\qquad
\vec e_n=
\begin{bmatrix}
0\\
0\\
\vdots\\
1
\end{bmatrix}.
$$

Because $T$ is linear, we can apply it to this linear combination:

$$
T(\vec{x})
=
T(x_1\vec e_1+x_2\vec e_2+\cdots+x_n\vec e_n)
$$

$$
=
x_1T(\vec e_1)+x_2T(\vec e_2)+\cdots+x_nT(\vec e_n).
$$

This is the key idea behind the transformation matrix.

## Transformation Matrix $M_T$

The transformation matrix is constructed by applying $T$ to each of the standard basis vectors.

The resulting vectors become the **columns** of $M_T$:

$$
M_T=
\begin{bmatrix}
|&|&&|\\
T(\vec e_1)&T(\vec e_2)&\cdots&T(\vec e_n)\\
|&|&&|
\end{bmatrix}.
$$

Therefore,

$$
T(\vec{x})=M_T\vec{x}.
$$

More explicitly,

$$
T(\vec{x})
=
\begin{bmatrix}
T(\vec e_1)&T(\vec e_2)&\cdots&T(\vec e_n)
\end{bmatrix}
\begin{bmatrix}
x_1\\
x_2\\
\vdots\\
x_n
\end{bmatrix}.
$$

### Finding the Transformation Matrix

To find $M_T$, calculate

$$
T(\vec e_1),\quad T(\vec e_2),\quad\ldots,\quad T(\vec e_n)
$$

and place these vectors as the columns of $M_T$.

This can be done geometrically, algebraically, or by using previously known matrices.

> [!Note]
> For a **square transformation matrix**, if
>
> $$
> \det(M_T)=0,
> $$
>
> then the transformation is **not invertible**.
>
> If
>
> $$
> \det(M_T)\neq0,
> $$
>
> then the transformation is invertible.
>
> The absolute value
>
> $$
> |\det(M_T)|
> $$
>
> represents the factor by which the transformation scales **area** in 2D or **volume** in 3D.
