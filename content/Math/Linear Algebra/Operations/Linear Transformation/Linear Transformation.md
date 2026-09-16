This is the equivalent of a function for regular algebra, except with a [[Matrix]]. Each linear transformation will have one corresponding output per input. 
>[!Note]
>The input to a linear transformation is called the range, and the output is called an image. 

### Goal of a Linear Transformation
The goal of a linear transformation is to express it in the form:
$$
T(\vec{x}) = M_T \vec{x},
$$
where:
- $T$ is the linear transformation,
- $M_T$ is the transformation matrix,
- $\vec{x}$ is the input vector.

---

### Representation of $\vec{x}$
The vector $\vec{x}$ can be expressed as a linear combination of the standard basis vectors $\vec{e}_1, \vec{e}_2, \dots, \vec{e}_n$:
$$
\vec{x} = \begin{bmatrix}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{bmatrix}
= x_1 \begin{bmatrix}
1 \\
0 \\
\vdots \\
0
\end{bmatrix}
+ x_2 \begin{bmatrix}
0 \\
1 \\
\vdots \\
0
\end{bmatrix}
+ \dots
+ x_n \begin{bmatrix}
0 \\
0 \\
\vdots \\
1
\end{bmatrix}
= x_1 \vec{e}_1 + x_2 \vec{e}_2 + \dots + x_n \vec{e}_n.
$$

---

### Transformation Matrix $M_T$
The transformation matrix $M_T$ is constructed by applying the linear transformation $T$ to each of the standard basis vectors $\vec{e}_1, \vec{e}_2, \dots, \vec{e}_n$. The resulting vectors $T(\vec{e}_1), T(\vec{e}_2), \dots, T(\vec{e}_n)$ form the columns of $M_T$:
$$
M_T = \begin{bmatrix}
T(\vec{e}_1) & T(\vec{e}_2) & \dots & T(\vec{e}_n)
\end{bmatrix}.
$$

---

### Applying the Transformation
The linear transformation $T(\vec{x})$ can then be expressed as:
$$
T(\vec{x}) = M_T \vec{x} = \begin{bmatrix}
T(\vec{e}_1) & T(\vec{e}_2) & \dots & T(\vec{e}_n)
\end{bmatrix}
\begin{bmatrix}
x_1 \\
x_2 \\
\vdots \\
x_n
\end{bmatrix}.
$$

## Finding the equation for a linear transformation
$T$ is realized by finding $T(\vec e_1)$, $T(\vec e_1)$...$T(\vec e_n)$ and put them in the columns of $M_T$. This can be done either geometrically, mathematically, or using previously known matrices. 

>[!Note]
>If the [[Determinant]] is 0, then the [[Linear Transformation]] is non-invertible. The [[Determinant]] of the [[Linear Transformation]] will also tell us by what factor the [[Linear Transformation]] changes the original [[Vector]].
