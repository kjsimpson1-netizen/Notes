---
aliases:
---
This is also known as the *inner product*. Whenever you do a dot product between two [[Vector]]s, you will get a [[Scalar]]. 
Letting $\vec a=(a_1,a_2,a_3 ...a_n)$ and $\vec b=(b_1,b_2,b_3 ...b_n)$, $\vec c$ be defined in the place $\mathbb{R}^n$ , the inner product will be defined as:
$$\begin{align*}
\vec a\cdot \vec b\equiv \langle\vec a,\vec b\rangle \equiv a_1b_1+a_2b_2+a_3b_3 ...a_nb_n
\end{align*}$$
which will be a [[Scalar]]. 
>[!Note]
>The dot product is also equal to the magnitude of the two vectors, multiplied together and multiplied by the cosine of $\theta$. This is also known as the cosine law
>$$\begin{align*}
\vec a\cdot \vec b&= ||\vec a||\;||\vec b||\cos\theta
\end{align*}$$

Using this, we can find the smallest angle $\theta$ between the two [[Vector]]s.
$$\begin{align*}
\theta &= \arccos\left(\frac{\vec a\cdot \vec b}{||\vec a||\;||\vec b||}\right)
\end{align*}$$
## Perpendicular
Another property of this is that if the dot of two vectors is equal to 0, then either one of the vectors is equal to 0, or these are [[Perpendicular]]. 
## Squaring
Another property of dot products is that when a [[Vector]] is dotted with itself, it is equal to it's [[Norm]] squared:
$$\begin{align*}
\vec a\cdot \vec a&= ||a||^2
\end{align*}$$
