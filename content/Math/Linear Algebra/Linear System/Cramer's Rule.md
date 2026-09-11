This is a method to solve a system of equations, where there are $n$ variables with $n$ equations, giving a $n\times n$ [[Matrix]]:
$
$
\begin{aligned}
\bf{A}&= \begin{pmatrix}
a_{11}&a_{12}&a_{13}&\cdots&a_{1n}\\
a_{21}&a_{22}&a_{23}&\cdots&a_{1n}\\
a_{31}&a_{32}&a_{33}&\cdots&a_{3n}\\
\vdots&\vdots&\vdots&\ddots&\vdots\\
a_{n1}&a_{n2}&a_{n3}&\cdots&a_{nn}
\end{pmatrix}
\end{aligned}
$
$
This will make up the matrix $\bf{A}$. The matrix $\bf{B}$ will be the constants of the equations:
$
$
\begin{aligned}
\bf{B}&= \begin{pmatrix}
b_1\\
b_2\\
b_3\\
\vdots\\
b_n
\end{pmatrix}
\end{aligned}
$
$
To solve for a given variable, you replace the $kth$ row of $\bf{A}$ with $\bf{B}$ and then find the [[Determinant]] of the matrix. For example, if we wanted to evaluate the variable in the 3rd row:
$
$
\begin{aligned}
\bf{A}_k&= \begin{vmatrix}
a_{11}&a_{12}&\cdots&b_{1}&\cdots&a_{1n}\\
a_{21}&a_{22}&\cdots&b_{2}&\cdots&a_{1n}\\
a_{31}&a_{32}&\cdots&b_{3}&\cdots&a_{3n}\\
\vdots&\vdots&\ddots&\vdots&\ddots&\vdots\\
a_{n1}&a_{n2}&\dots&b_{n}&\cdots&a_{nn}
\end{vmatrix}
\end{aligned}
$
$
We then divide the [[Determinant]] of $\bf{A}_k$ by the original [[Determinant]] of $\bf{A}$ to determine the value of $x_3$:
$
$
\begin{aligned}
x_k&= \frac{\det(\bf{A}_k)}{\det(\bf{A})}
\end{aligned}
$
$
>[!Warning]
>This assumes that $\det(\bf{A})\neq0$

