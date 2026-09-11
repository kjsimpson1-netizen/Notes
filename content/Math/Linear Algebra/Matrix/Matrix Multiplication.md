### Matrix Multiplication Condition
[[Matrix]] multiplication is defined **only when the number of columns in the first matrix** ($A$) **matches the number of rows in the second matrix** ($B$). If $A$ is an $m \times n$ matrix and $B$ is an $n \times p$ matrix, their product $C = AB$ will be an $m \times p$ matrix. This can be expressed as $AB\equiv\langle A,B\rangle$

---

### Formula for Matrix Multiplication
Each element $c_{ij}$ of the resulting matrix $C$ is computed as the **dot product** of the $i$-th row of $A$ and the $j$-th column of $B$. Mathematically, this is expressed as:
$$
c_{ij} = \sum_{k=1}^{n} a_{ik}\cdot b_{kj}
$$
$$
A = \begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}, \quad
B = \begin{bmatrix}
b_{11} & b_{12} & \cdots & b_{1p} \\
b_{21} & b_{22} & \cdots & b_{2p} \\
\vdots & \vdots & \ddots & \vdots \\
b_{n1} & b_{n2} & \cdots & b_{np}
\end{bmatrix}, \quad
C = AB = \begin{bmatrix}
c_{11} & c_{12} & \cdots & c_{1p} \\
c_{21} & c_{22} & \cdots & c_{2p} \\
\vdots & \vdots & \ddots & \vdots \\
c_{m1} & c_{m2} & \cdots & c_{mp}
\end{bmatrix}
$$
>[!Note]
>The order of the matrices being multiplied cannot switch as this operation is not communicative

### Dimensions
This also has the property of changing the dimensions of the vectors. If $\vec x$ is in $n$ dimensional space, and $A$ is in $m$ dimensional space, then $b$ will be in $m$ dimensional space. 
