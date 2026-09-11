If the [[Matrix]] is an Invertible Matrix and the [[Matrix]] is a [[One-to-One Linear Transformations]], then we can find it's inverse matrix. The notation of an inverse matrix equation is:
$
\begin{aligned}
\vec x&= \bf{A}^{-1}\vec b
\end{aligned}
$
## Invertibility
In order for a [[Matrix]] to be invertible, the matrix must:
1. Have a non-zero [[Determinant]]
2. No 2 rows or columns can have [[Linear Independence]]
3. The matrix must be square ($n\times n$)
4. It must be a [[One-to-One Linear Transformations]]
5. The [[Reduced Row Echelon Form]] of $\bf A$ must be the [[Identity Matrix]]
>[!Note]
>If there is a [[Matrix Multiplication]] and both of the matrices are invertible, then the inverse [[Matrix Multiplication]] of the two is also invertible
## Finding the Inverse
There are two different ways to find the inverse matrix, either using a formula or [[Gaussian Elimination]]. 
### [[Gaussian Elimination]]
We can set this up as the following:
$
\begin{aligned}
\begin{bmatrix}
A&|&I
\end{bmatrix}\longrightarrow \begin{bmatrix}
I&|&A^{-1}
\end{bmatrix}
\end{aligned}
$
This states that we can set the [[Linear Transformation]] matrix equal to the [[Identity Matrix]] of the same size, then use [[Gaussian Elimination]] to get the original [[Linear Transformation]] into [[Reduced Row Echelon Form]] and then the remainder on the right side is the inverse matrix
### Formula
The formula for the inverse of a [[Matrix]] is:
$
\begin{aligned}
\mathbf{A^{-1}}&= \left(\frac1{\det(A)}\right)C^T
\end{aligned}
$
Where $C^T$ is the transpose of the [[Cofactor]] of each entry. 
### $2\times2$ matrix Formula
We can derive this using the method above, however with general variables ($a,b,c,d$):
$
\begin{aligned}
\bf{A}^{-1}&= \frac1{\det A}\begin{bmatrix}
d&-b \\ -c&a
\end{bmatrix}
\end{aligned}
$
## Verifying
After we have found the inverse matrix, we can then use [[Matrix Multiplication]] to ensure that the the product is the [[Identity Matrix]].
$
\begin{aligned}
\bf{AA}^{-1}&= \bf{I}
\end{aligned}
$
