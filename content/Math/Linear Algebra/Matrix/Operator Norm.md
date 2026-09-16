The operator norm is defined by :
$$
\begin{aligned}
||A||=\max_{x\neq0}\frac{||Ax||}{||x||}
\end{aligned}
$$
This is the [[Matrix]] analog of the [[Euclidian Norm|Euclidian Norm]] for  a [[Vector]]. Some properties of the operator norm are:
1. $$
\begin{aligned}
||A||&= \max_{||x||=1}||Ax||
\end{aligned}
$$
This tells us that it is just a rotation i.e. it lies on the unit circle. 
2. If $A$ is a square [[Matrix]] and has an [[Inverse Matrices]], this means that the following is true:
   $$
\begin{aligned}
||A^{-1}||&= \frac1{\min||Ax||}
\end{aligned}
$$

>[!Note]
>$$
\begin{aligned}
||D||=\max|d_i|
\end{aligned}
$$
Where $D$ is defined to be a [[Diagonal Matrices]]
3. In order to be an operator norm, the following must also hold:
   $$
\begin{aligned}
||AB||_*\le||A||_*||B||_*
\end{aligned}
$$
