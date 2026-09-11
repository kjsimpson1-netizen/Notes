This is a subset of [[Linear Algebra]], however instead of just regular [[Vector|Vectors]], this is a special kind that is broken in something called bra's ,$\bra{x}$, and ket's, $\ket x$ (a play on words of the bracket). These forms of [[Vector|Vectors]] also have all the operations, such as [[Dot Product|Inner Product]], [[Outer Product]], etc. The inner product is represented by $\braket{x|x}$, and the outer product is given by $\ket{x}\bra{x}$. 
>[!Warning]
>Unlike regular [[Dot Product]], where $(-\hat i)\cdot(\hat i)=-1$, $\braket{+x|-x}=0$

## Bra's and Ket's
If we are given a ket, $\ket{x}$, in order to find it's bra, we take the transpose conjugate of the ket. 
$$
\begin{aligned}
\ket{x}&\equiv  \begin{bmatrix}
u_1\\u_2
\end{bmatrix}\\
\bra{x}&\equiv \begin{bmatrix}
u_1^*&u_2^*
\end{bmatrix}
\end{aligned}
$$
>[!Note]
>An important property of a bra and it's respective ket is that the inner product will always give 1 (assuming that it's normalized).
## Probability Amplitudes
When we take the inner product of two states, we will get the probability amplitude. In order to find the actual probability, we will have to square the probability amplitude. 