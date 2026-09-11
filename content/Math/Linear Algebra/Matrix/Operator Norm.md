The operator norm is defined by :
$$\begin{align*}
||A||=\max_{x\neq0}\frac{||Ax||}{||x||}
\end{align*}$$
This is the [[Matrix]] analog of the [[Norm|Euclidian Norm]] for  a [[Vector]]. Some properties of the operator norm are:
1. $$\begin{align*}
||A||&= \max_{||x||=1}||Ax||
\end{align*}$$
This tells us that it is just a rotation i.e. it lies on the unit circle. 
2. If $A$ is a square [[Matrix]] and has an [[Inverse Matrices]], this means that the following is true:
   $$\begin{align*}
||A^{-1}||&= \frac1{\min||Ax||}
\end{align*}$$

>[!Note]
>$$\begin{align*}
||D||=\max|d_i|
\end{align*}$$
Where $D$ is defined to be a [[Diagonal Matrices]]
