Whenever the function feels like it has the form $\frac00$ or $\frac{\infty}{\infty}$, then we can general factor it to find out what the function approaches, rather than finding the actual value. If this doesn't work, we will have to apply [[L'Hopitals Rule]].
$$
\begin{aligned}
\lim_{x\rightarrow 2}f(x)&= \lim_{x\rightarrow 2}\frac{x-2}{x^2+x-6}\\
&= \lim_{x\rightarrow 2}\frac{x-2}{(x+3)(x-2)}\\
&= \lim_{x\rightarrow 2}\frac{\cancel{x-2}}{(x+3)\cancel{(x-2)}}\\
&= \lim_{x\rightarrow 2}\frac1{x+3}\\
&= \frac1{(2)+3}\\
&= \frac15
\end{aligned}
$$

>[!Note]
>If $f(x)=g(x)$ at all values except $x=a$, then:
>$$
\begin{aligned}
\lim_{x\rightarrow a}f(x)=\lim_{x\rightarrow a}g(x)
\end{aligned}
$$
Provided it exists


