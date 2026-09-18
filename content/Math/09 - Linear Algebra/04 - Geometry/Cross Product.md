This is the product of any two vectors with the "cross" multiplication symbol:
$$
\begin{aligned}
\vec a\times\vec b&= \vec c
\end{aligned}
$$
The cross product gives us a vector that is [[Perpendicular]] to the original two vectors. 
>[!Warning]
>The order of the vectors cannot be changed, or:
>$$
\begin{aligned}
\vec a \times &\vec b\neq \vec b\times \vec a
\end{aligned}
$$
When this is done, it is equal to $-\vec b\times\vec a$

This is very similar to the [[Determinant]] of 3D [[Matrix]]. We can calculate this using the following
$$
\begin{aligned}
\vec a&= \begin{pmatrix}
a_1\\
a_2\\
a_3
\end{pmatrix}&\vec b&= \begin{pmatrix}
b_1\\
b_2\\
b_3
\end{pmatrix}\\
&&\vec a\times \vec b&= \begin{vmatrix}
\hat i&\hat j&\hat k\\
a_1&a_2&a_3\\
b_1&b_2&b_3
\end{vmatrix}
\end{aligned}
$$
>[!Note]
>The length or the [[Euclidean Norm]] of [[Vector]] $\vec c$ is the following:
>$$
\begin{aligned}
||\vec a\times \vec b||&= ||\vec a||||\vec b||\sin\theta\\
\end{aligned}
$$
This will also be the same as the area of a parallelogram with sides $\vec a$ and $\vec b$

>[!Warning]
Do not use this to calculate the angle, as the $\arcsin$ function doesn't work well with angles greater than $\frac12\pi$, as it will give the smallest angle between $\vec a$ and $\vec b$
## Properties
1. All three of the vectors must be an element of $\mathbb{R}^3$
2. The product of the cross product is perpendicular to the two factors
3. As long as we keep the order of the variables the same, the following is true:
   $$
\begin{aligned}
\vec a\cdot (\vec b\times \vec c)&= (\vec a\times \vec b)\cdot c=\vec b(\vec c\times \vec a)
\end{aligned}
$$
>[!Note]
>This is also equal to:
>$$
\begin{aligned}
(\vec a\times \vec b)\cdot \vec c&= \begin{vmatrix}
a_1&a_2&a_3\\
b_1&b_2&b_3\\
c_1&c_2&c_3
\end{vmatrix}
\end{aligned}
$$
4. The cross product is equal to 0 if either [[Vector]] is 0, or if the two vectors are parallel. 