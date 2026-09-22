This is a type of [[10 - Interpolation]] that uses a sum of polynomials to fit a given set of data. For a data set with $d+1$ data points, we can **always** make a polynomial of degree $n$ that will fit these date points with the function. The function is given by:
$$
\begin{aligned}
P_d(x)=c_0+c_1t+c_2t^2+...c_dt^d
\end{aligned}
$$
Such that $P_d(t_k)=y_k,k\in\mathbb{N}\in[0,d]$. We can rewrite this in [[Matrix]] form $Ac=y$ as:
$$
\begin{aligned}
A=\begin{bmatrix}
1&t_0&\cdots&t_0^d\\
1&t_1&\cdots&t_0^1\\
\vdots&\vdots&\ddots&\vdots\\
1&t_d&\cdots &t_d^d
\end{bmatrix},\quad c=\begin{bmatrix}
c_0\\c_1\\c_2\\\vdots\\c_d
\end{bmatrix},\quad y=\begin{bmatrix}
y_0\\y_1\\y_2\\\vdots\\y_d
\end{bmatrix}
\end{aligned}
$$
The [[Matrix]] $A$ is called the [[Vandermonde Matrix]]. 
>[!Note]
>The [[Condition Number]] of the [[Vandermonde Matrix]] is very large, and therefore this method can introduce relatively large [[Relative Error]]

