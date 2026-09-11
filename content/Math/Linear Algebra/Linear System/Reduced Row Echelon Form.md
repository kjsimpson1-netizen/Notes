This is another method for [[Linear System]]. This is very similar to [[Row Echelon Form]], however without any non-zero values in the non-pivotal positions. When the reduced row echelon form is applied to the matrix, it will make it look like:
$$\begin{align*}
\bf{A}&= \begin{bmatrix}
1&0&0&\cdots&0&\text{Answer}_1\\
0&1&0&\cdots&0&\text{Answer}_2\\
0&0&1&\cdots&0&\text{Answer}_3\\
\vdots&\vdots&\vdots&\ddots&\vdots&\vdots\\
0&0&0&\cdots&1&\text{Answer}_n
\end{bmatrix}
\end{align*}$$
With the last column being the answer to the $nth$ variable. In this form any column that has no leading one, it is a parameter, and therefore the amount of columns without the leading ones is equivalent to the amount of dimensions.