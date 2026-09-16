This is used when the actual [[Definite Integral]] is not known and therefore the approximation cannot be compared to any value. Therefore, and equation is needed to put a bound on how large the error can be. 
## Trapezoidal
The equation for this is with the trapezoidal method is:
$$
\begin{aligned}
E_M=\left|\int_a^bf(x)dx-T_n(f)\right|&\le\frac M{12}\frac{(b-a)^3}{n^2}
\end{aligned}
$$
The value for $M$ is a value such that $|f''(x)|\le M$ in $[a,b]$.
## Simpsons Rule
The equation for the error on [[Simpson's Rule]] is:
$$
\begin{aligned}
E_S=\left|\int_a^bf(x)dx-S_n(f)\right|&\le\frac L{12}\frac{(b-a)^5}{n^4}
\end{aligned}
$$
The $n$ value must be even for this expression. The term $L$ is the largest that the fourth [[Derivative]] of the function can be on the given interval. 

