  The [[Undetermined Coefficients]] method does not always work for functions where the [[Derivative|Derivatives]] don't behave nicely (i.e. follow a nice pattern). This works for equations of the following form:
$$\begin{align*}
y''+p(x)y'+q(x)y=f(x)
\end{align*}$$
We can also use [[Integration Factor Method]] to solve this form. However, this is just another method. If we can first solve the [[Homogeneity|Homogenous]] form, we can then do the same method as [[Undetermined Coefficients]], however with functions instead.  
We first have to find the solution to the complimentary solution, $y_c$, being $y_c=C_1y_1+C_2y_2$. From here we can get the following equations:
$$\begin{align*}
u'_1y_1+u'_2y_2&= 0\\
u'_1y'_1+u'_2y'_2&= f(x)
\end{align*}$$
From this point we just have to solve this system of equations to find our function $u$ by integrating $u'_1$ and $u'_2$, and then plugging the answers back into the form:
$$\begin{align*}
y_p&= u_1y_1+u_2y_2
\end{align*}$$
