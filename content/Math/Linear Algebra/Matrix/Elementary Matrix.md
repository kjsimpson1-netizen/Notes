---
aliases:
  - Elemental Matrices
---
This is an [[Identity Matrix]] where there has been a singular row operation done on it such that there is one entry that is different. This is shown by the letter $E$.
$
\begin{aligned}
E&= \begin{bmatrix}
1&&&&\\
&\ddots&&&\\
&&\ddots\\
&c&&\ddots\\
&&&&1
\end{bmatrix}
\end{aligned}
$
>[!Note]
>When multiplying a [[Matrix]] by $E$ with a row operation done so that it's $c_{ij}$ entry differs from the [[Identity Matrix]], this is equivalent to adding $c$ times the $i$th row to the $j$th row in [[Gaussian Elimination]].

### Inverse Matrix
Also, the [[Inverse Matrices]] of an elementary matrix is the same, however with the sign of the $c_{ij}$ entry. 
$
\begin{aligned}
E&= \begin{bmatrix}
1&&&&\\
&\ddots&&&\\
&&\ddots\\
&-c&&\ddots\\
&&&&1
\end{bmatrix}
\end{aligned}
$
### Matrix Multiplication
When [[Matrix Multiplication]] is done upon two elementary matrices, we can just replace the relevant entries
$
\begin{aligned}
E_1E_2&= \begin{bmatrix}
1&&&&\\
&\ddots&&&\\
&&\ddots\\
&c_1&&\ddots\\
&&&&1
\end{bmatrix}
\begin{bmatrix}
1&&&&\\
&\ddots&&&\\
&c_2&\ddots\\
&&&\ddots\\
&&&&1
\end{bmatrix}= \begin{bmatrix}
1&&&&\\
&\ddots&&&\\
&c_2&\ddots\\
&c_1&&\ddots\\
&&&&1
\end{bmatrix}
\end{aligned}
$
