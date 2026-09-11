  This is a more accurate version of a [[Taylor Polynomials]], where the [[Taylor Polynomials]] are taken as $n\rightarrow\infty$.
$$
\begin{aligned}
f(x)&= \sum_{k=0}^{\infty}\frac{f^{(k)}(a)}{k!}\cdot(x-a)^k
\end{aligned}
$$
Giving us a perfect approximation of the function. In order for the Taylor series to be taken, the function must be infinitely differentiable at $x=a$ and have a non-zero [[Radius of Convergence]]. These also have the property of allowing us to calculate the nth order derivative, as we can represent the function with both the Taylor series and the [[Power Series]], and then solve for the desired derivative.
Another useful application is computing the asymptotic behavior, as the Taylor series often has an asymptote that is easier to see than the function. 
$$
\begin{aligned}
\ln(x) &= \sum_{n=1}^\infty (-1)^{n+1} \frac{(x - 1)^n}{n}, && \text{(centered at } x = 1,\ |x - 1| < 1) \\[1em]

\frac{1}{x} &= \sum_{n=0}^\infty (-1)^n (x - 1)^n, && \text{(centered at } x = 1,\ |x - 1| < 1) \\[1em]

e^x &= \sum_{n=0}^\infty \frac{x^n}{n!}, && \text{(centered at } x = 0,\ \text{entire domain)} \\[1em]

\arctan(x) &= \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{2n+1}, && \text{(centered at } x = 0,\ |x| \leq 1) \\[1em]

\sin(x) &= \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!}, && \text{(centered at } x = 0) \\[1em]

\cos(x) &= \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}, && \text{(centered at } x = 0)
\end{aligned}
$$
