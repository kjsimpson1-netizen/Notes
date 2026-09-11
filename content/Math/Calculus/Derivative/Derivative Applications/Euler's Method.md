This is an approximation of the function similar to [[Taylor Polynomials]], using the tangent line and then stepping along it a predetermined amount, and doing another [[Tangent Line]]
$$
$$
\begin{aligned}
y_1&= y_0+f(t_0,y_0)\cdot h\\
y_2&= y_1+f(t_1,y_1)\cdot h\\
&...\\
y_{m+1}&= y_n+f(t_n,y_n)\cdot h\\
\hline \\
\frac{dy}{dt}&= f(t,y)\\
h&= \Delta x\\
x_1&= x_0+h\\
x_{n+1}&= x_n+h
\end{aligned}
$$
$$
The $h$ is a chosen value that we choose for the step size along the tangent line. However, if the graph is concave up, then the Euler's approximation will always underestimate, and if it is concave down, then the method will always overestimate
>[!Warning]
>There are error's in this method. 
>1. The further from the starting point, the larger the error. 
>2. The more steps from the starting point, the greater the error
>3. A greater $f''$ will cause a greater fluctuation

