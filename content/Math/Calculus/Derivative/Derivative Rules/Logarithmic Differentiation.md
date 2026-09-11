We use logarithms because products are slower and take more work, whereas sums are easy and quick. We can see why this works using [[Chain Rule]]:
$$\begin{align*}
\frac d{dx}\Big[\log(f(x))\big]&= \frac{f'(x)}{f(x)}
\end{align*}$$
We can use this to take faster derivatives
$$\begin{align*}
f(x)&= (x^2+7x+8)^9\\
\log(f(x))&= 9\log(x^2+7x+8)\\
\frac{f'(x)}{f(x)}&= 9\cdot\frac{2x+7}{x^2+7x+8}
\end{align*}$$
We can then solve this for $f'(x)$
$$\begin{align*}
f'(x)&=\frac{9(2x+7)\cdot f(x)}{x^2+7x+8}\\
&= 9(2x+7)\cdot(x^2+7x+8)^8
\end{align*}$$


$$\begin{align*}
f(x)&= \frac{12e^{5-t}}{(1+e^{5-t})^2}\\
f'(x)&= \frac{-12e^{5-t}(1+e^{5-t})^2-2(1+e^{5-t})(-e^{5-t})12e^{5-t}}{(1+e^{5-t})^4}\\
0&= -12e^{5-t}(1+e^{5-t})^2-2(1+e^{5-t})(-e^{5-t})12e^{5-t}\\
&= -12e^{5-t}((1+e^{5-t})^2+2(1+e^{5-t})(-e^{5-t}))\\
\\
&= ((1+e^{5-t})^2-2(1+e^{5-t})(e^{5-t}))\\
&= (1+e^{5-t})((1+e^{5-t})-2e^{5-t})\\
&= 1-e^{5-t}\\
1&= e^{5-t}\\
0&= 5-t\\
t&= 5
\end{align*}$$