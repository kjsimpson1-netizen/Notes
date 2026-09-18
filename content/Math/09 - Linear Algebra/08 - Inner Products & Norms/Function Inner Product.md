This is the [[Inner Product]] between two functions. We can derive this qualitatively using the [[Vector]] [[Dot Product]]. Give two vectors:$$
\begin{aligned}
\vec a=\begin{bmatrix}
a_1\\a_2\\a_3\\\vdots\\a_n
\end{bmatrix}&&
\vec b=\begin{bmatrix}
b_1\\b_2\\b_3\\\vdots\\b_b
\end{bmatrix}
\end{aligned}
$$
Taking their [[Dot Product]] gives:
$$
\begin{aligned}
\vec a\cdot\vec b=\sum_{i=1}^na_ib_i
\end{aligned}
$$
Taking the same idea for an integral, if we want to take the sum of the product at all outputs of two functions, $f(x),g(x)$, we could express this as:
$$
\begin{aligned}
\langle f(x),g(x)\rangle=\sum_{i=1}^nf(x_i)g(x_i)\Delta x
\end{aligned}
$$
When we take this to a continuous level, we get:
$$
\begin{aligned}
\braket{f(x),g(x)}&= \int_0^Lf(x)g(x)dx
\end{aligned}
$$
>[!Note]
>We can also add a **weight function** to this, in order to give the [[Weighted Inner Product]]