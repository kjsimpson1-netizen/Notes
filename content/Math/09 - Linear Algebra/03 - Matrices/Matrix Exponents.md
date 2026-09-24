A [[Matrix]] as an exponent doesn't have a physical meaning. It only acts as a definition, and it is only useful when we use the [[Taylor Series]] to represent it. Given a the [[Taylor Series]] for the exponential:$$
\begin{aligned}
e^x &= \sum_{n=0}^\infty \frac{x^n}{n!}
\end{aligned}
$$Replacing the $x$ with a [[Matrix]]$$
\begin{aligned}
e^A=\sum_{n=0}^\infty \frac{A^n}{n!}
\end{aligned}
$$From here, this represents a repeated application of the [[Matrix]]. The most useful version of this is when it is multiplied by one of its [[Eigenvector|Eigenvectors]], as then we can pull the [[Matrix]] out by doing the following$$
\begin{aligned}
U(s)\ket{\phi}&= \exp(-i\hat G s)(c_1\ket{\lambda_1}+c_2\ket{\lambda_2})\\
&= \left(\sum_{n=1}^\infty\frac{(-i\hat Gs)^n}{n!}\right)(c_1\ket{\lambda_1}+c_2\ket{\lambda_2})\\
&= c_1\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\hat G^n\ket{\lambda_1}\right)+
c_2\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\hat G^n\ket{\lambda_2}\right)\\
&= c_1\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\lambda_1\ket{\lambda_1}\right)+
c_2\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\lambda_2\ket{\lambda_2}\right)\\
&= c_1\exp(-is\lambda_1)+c_2\exp(-is\lambda_2)
\end{aligned}
$$From this point, we can re express this in any basis of choosing. 