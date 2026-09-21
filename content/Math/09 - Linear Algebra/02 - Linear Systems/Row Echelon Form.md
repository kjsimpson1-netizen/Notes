This is the form of which you want to get for [[Math/09 - Linear Algebra/02 - Linear Systems/Linear System]]. The row echelon form, or REF, looks like:
$$
\begin{aligned}
\begin{bmatrix} 1 & * & * & * & \dots & * \\ 0 & 1 & * & * & \dots & * \\ 0 & 0 & 1 & * & \dots & * \\ 0 & 0 & 0 & 1 & \dots & * \\ \vdots & \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & 0 & \dots & 1 \end{bmatrix}
\end{aligned}
$$
Where each $1$ represents the variable that has been solved for, and the $*$ is any non-zero value. oThis form can be achieved using [[Gaussian Elimination]] to get rid of the values under the staircase. 
>[!Note]
>If there is a row of all zeroes, then this is a free variable and can be set equal to any value, or substituted with $t$ and then back substitute to find the [[Parametric Formula]] of a line in 3 dimensional space

