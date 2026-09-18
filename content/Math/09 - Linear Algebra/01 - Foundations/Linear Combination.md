---
aliases:
  - Linear Combinations
---
## Linear Combinations

A **linear combination** is when a set of [[Vector]]s are multiplied by [[Scalar]]s and then summed together.

$$
\vec b=s_1\vec a_1+s_2\vec a_2+\cdots+s_m\vec a_m,
\qquad m\in\mathbb N
$$

The scalars $s_1,s_2,\ldots,s_m$ determine how much of each vector is used in the linear combination.

## Standard Basis Vectors

This is the same idea as [[Cartesian Coordinates]], but instead of using the unit vectors $\hat i,\hat j,\hat k$, we use the letter $e$ with a subscript representing which coordinate direction it refers to.

For example:

$$
\begin{aligned}
\vec e_1&=(1,0,0,\ldots)\\
\vec e_2&=(0,1,0,\ldots)\\
\vec e_3&=(0,0,1,\ldots)
\end{aligned}
$$

These are called the **standard basis vectors**.

Any vector can be written as a linear combination of the standard basis vectors. For example:

$$
\vec v=(v_1,v_2,v_3)
$$

can be written as

$$
\vec v=v_1\vec e_1+v_2\vec e_2+v_3\vec e_3.
$$

Thus, the coordinates of a vector are simply the [[Scalar]]s multiplying the corresponding basis vectors.

> [!Note]
> A set of vectors is **linearly independent** if none of the vectors can be written as a linear combination of the others.
>
> Equivalently, the only solution to
>
> $$
> s_1\vec a_1+s_2\vec a_2+\cdots+s_m\vec a_m=\vec 0
> $$
>
> is
>
> $$
> s_1=s_2=\cdots=s_m=0.
> $$
>
> If one vector **can** be written as a linear combination of the others, then the vectors are [[Linear Independence|linearly dependent]].
