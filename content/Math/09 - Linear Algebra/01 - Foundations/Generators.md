A generator produces a [[Linear Transformation]] when repeatedly applied. These generators will be a [[Hermitian Matrix]] and [[Unitary Matrices]]. In order for these to be applied, they will be exponentiated, letting $G$ be the [[Generators]] and the $U$ being the [[Linear Transformation]]:
$$
\begin{aligned}
\hat U(\theta)=\exp(-i\hat G\theta)
\end{aligned}
$$
>[!Note]
>The generator being in the exponent doesn't have a physical meaning. It only acts as a definition, and it is only useful when we use the [[Taylor Series]] to represent it. 

These become useful when we apply them to a state, particularly when the state that is being represented is expressed in the eigen basis of the generator (using the [[Spectral Theorem]]. We can show this as:
$$
\begin{aligned}
U(s)\ket{\phi}&= \exp(-i\hat G s)(c_1\ket{\lambda_1}+c_2\ket{\lambda_2})\\
&= \left(\sum_{n=1}^\infty\frac{(-i\hat Gs)^n}{n!}\right)(c_1\ket{\lambda_1}+c_2\ket{\lambda_2})\\
&= c_1\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\hat G^n\ket{\lambda_1}\right)+
c_2\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\hat G^n\ket{\lambda_2}\right)\\
&= c_1\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\lambda_1\ket{\lambda_1}\right)+
c_2\left(\sum_{n=1}^\infty\frac{(-is)^n}{n!}\lambda_2\ket{\lambda_2}\right)\\
&= c_1\exp(-is\lambda_1)+c_2\exp(-is\lambda_2)
\end{aligned}
$$
From this point, we can re express this in any basis of choosing. 

