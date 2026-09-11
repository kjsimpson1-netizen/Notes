These are when a base is raised to a square [[Matrix]] power, $e^{At}$. We can calculate these by:
$
$
\begin{aligned}
e^{At}&= TDT^{-1}
\end{aligned}
$
$
Where the the nth column of $T$ is the nth [[Eigenvalues|Eigenvectors]] and $D$ is:
$
$
\begin{aligned}
D&= \begin{bmatrix}
e^{\lambda_1t}&0&0&\dots&0\\0&e^{\lambda_2t}&0&\cdots&0\\0&0&e^{\lambda_3t}&\dots&0\\
\vdots&\vdots&\vdots&\ddots\\0&0&0&&e^{\lambda_nt}
\end{bmatrix}_{n\times n}
\end{aligned}
$
$
>[!Note]
>When we raise a base to the power of a [[Matrix]], the answer will be a [[Matrix]] of the same dimensions as the exponent