This is used for when the function that we want to take the [[Derivative]] of has algebra contained inside of another term, or a composite term. 
E.g. $e^{2x}$
## Formula
$$\begin{align*}
\frac{dy}{dx}&= \frac{dy}{du}\cdot\frac{du}{dx}\\
\\
\frac d{dx}\Big[f(g(x))\Big]&= f'(g(x))\cdot g'(x)
\end{align*}$$
For this, all you have to do is calculate the [[Derivative]] of the outside piece, and then multiply by the part inside, while not changing what is inside of the operator.
## Example
$$\begin{align*}
&&h(x)&= e^{2x}\\
\\
\hline\\
&&f(t)&=e^t&\textcolor{red}{\text{Values Needed}}\\
&&f'(t)&= e^t\\
\\
&&g(t)&= 2x\\
&&g'(t)&= 2\\
\\
\hline\\
&&h'(x)&=f'(g(x))\cdot g'(x)&\textcolor{red}{\text{Chain Rule Definition}}\\
&\implies&&= e^{2x}\cdot2\\
&\implies&&= 2e^{2x}
\end{align*}$$
We can see that the function will "spit out" the derivative of the outside part. 