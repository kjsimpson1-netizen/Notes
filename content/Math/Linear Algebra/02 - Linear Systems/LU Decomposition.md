This is an
other method to solve a [[Linear System]]. It uses [[Gaussian Elimination]] and [[Elementary Matrix|Elemental Matrices]] in order to solve the system. This form of solving a [[Linear System]] is most useful when using the same coefficient [[Matrix]], as we can reuse the $L$ and $U$ [[Matrix|Matrices]]. The steps are:
1. Reduce the given [[Matrix]] $A$ into a [[Upper Triangular Matrix]] through [[Gaussian Elimination]], and recording each of the steps done in a [[Lower Triangular Matrix]] 
2. From here, we can take the given [[Linear System]] $A\vec x=\vec b$ and we can solve by first letting $L\vec y=\vec b$, and from here we can solve the equation $U\vec x=\vec y$
This will give us the following equality:
$$
\begin{aligned}
A&= LU
\end{aligned}
$$
### Properties
We have that the [[Rank]] of the two triangular [[Matrix|Matrices]] are both equivalent i.e. $\text{Rank}(A)=\text{Rank}(U)$
>[!Warning]
>Not all [[Matrix|Matrices]] have valid LU decompositions, for example the [[Matrix]]:
>$$
\begin{aligned}
D=\begin{bmatrix}
0&1\\1&0
\end{bmatrix}
\end{aligned}
$$
Does not have a LU decomposition

