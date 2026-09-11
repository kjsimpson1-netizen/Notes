These can be calculated by multiplying the base length of the parallelogram by the height. However, we can also express this in terms of the [[Vector]] that make it up, $\vec a$ and $\vec b$. First we can find the height by finding the $\vec a_\perp$ component of $\vec{b}$, then multiplying this by $\vec{a}$. Since this becomes the definition of the [[Dot Product]], we can write this as the following. 
![[ParallelogramArea.png|600]]
## 2 Dimensions
$
\begin{aligned}
A&= (\text{Base})(\text{Height})\\
&= \big(||\vec a||\big)\big(||\vec b||\sin\theta\big)
\end{aligned}
$
Since $\sin\theta=\cos(\frac12\pi-\theta)$, we can rewrite it as:
$
\begin{aligned}
&= |\vec a||||\vec b||\cos\left(\frac\pi2-\theta\right)
\end{aligned}
$
and since the term $||\vec b||\cos\left(\frac\pi2-\theta\right)$ is the same thing as $\vec a_\perp$, we can rewrite it as the following, using [[Perpendicular]]:
$
\begin{aligned}
&= ||\vec a|||||\vec a_\perp||
\end{aligned}
$
and use this to get the following:
$
\begin{aligned}
\boxed{A= \big|a_1b_2-a_2b_1\big|}
\end{aligned}
$

Since this is the exact same result that we would get from the [[Determinant]] of the two [[Vector]], we can also use the absolute value of the determinant to find the area, or:
$
\begin{aligned}
A_\text{pgram}&= \text{abs}\left(\begin{vmatrix}
a_1&a_2\\
b_1&b_2
\end{vmatrix}\right)
\end{aligned}
$

>[!Note]
>This also works for a parallelepiped (a 3 dimensional shape with it's sides all being parallelograms), just with a 3 by 3 matrix rather than a 2 by 2 matrix, using the [[Cross Product]] as necessary
>$
\begin{aligned}
\boxed{V= |\vec a\cdot(\vec b\times \vec c)|}
\end{aligned}
$

## 3 Dimensions
We can do the same with finding the area of a parallelogram in 3 dimensions, using the following equation:
$
\begin{aligned}
\boxed{A_\text{pgram}= ||\vec a\times \vec b||}
\end{aligned}
$
