The rank of a [[Matrix]] is defined as the number of rows in an [[Matrix]] that are nonzero in the [[Row Echelon Form]]. In order to see the rank of a [[Matrix]], we must first have the [[Matrix]] in [[Row Echelon Form]]. For example, the following is a rank 3 [[Matrix]], because they have 3 nonzero rows:
$
$
\begin{aligned}
\text{Rank}[A|\vec b]= \text{Rank}\begin{bmatrix}
1 & 2 & 3 & \vert & 4 \\
0 & 1 & 5 & \vert & 6 \\
0 & 0 & 3 & \vert & 8
\end{bmatrix}=3
\end{aligned}
$
$

> [!Note]  
> There are three possibilities we can see from the rank and the number of variables:  
> 1. **Unique Solution**: If the rank of $A$ is equal to the rank of $\vec{b}$, and this rank is also equal to the number of variables, then the system has a unique solution.  
> 2. **No Solution**: If the rank of $A$ is less than the rank of $\vec{b}$, then the system has no solution.  
> 3. **Infinite Solutions**: If the rank of $A$ is equal to the rank of $\vec{b}$, but the rank is less than the number of variables, then the system has infinitely many solutions.


