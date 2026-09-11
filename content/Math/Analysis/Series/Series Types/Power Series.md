A power series is when a [[Series]] is taken with $x$ raised to the nth power. This is shown by:
$
\begin{aligned}
\sum_{n=0}^\infty A_n(x-c)^n
\end{aligned}
$
These are very useful in [[Taylor Series]]. It is also sometimes useful to rewrite a power series as a [[Geometric Series]]:
$
\begin{aligned}
\sum_{n=0}^\infty\frac1{1-x}&= \sum_{n=0}^\infty x^n
\end{aligned}
$
## Calculus
In order to perform calculus on a power series, we must first confirm that it converges. This can usually be done using the [[Ratio Test]]. If the series converges, we can then use regular derivatives and integral rules on the series:
$
\begin{aligned}
S'(x)&= \sum_{n=1}^{\infty}nA_n(x-c)^{n-1}\\
\int S(x)dx&= \sum_{n=0}^{\infty}\frac1{n+1}A_n(x-c)^{n+1}+C
\end{aligned}
$
Although this seems arbitrary, this has important uses in [[Taylor Series]] in easily calculating the nth derivatives. 
>[!Note]
>When doing arithmetic with multiple series, use the [[Radius of Convergence]] of the series with the smaller [[Radius of Convergence]], as even though the larger one may be well behaved, the small one won't be

We can use the following power series as "building blocks" to make more complex power series.
## Known Power Series
$$
\begin{aligned}
\ln(x) &= \sum_{n=1}^\infty (-1)^{n+1} \frac{(x - 1)^n}{n},  &|x - 1| < 1 \\[1em]

\frac{1}{1 - x} &= \sum_{n=0}^\infty x^n, & |x| < 1 \\[1em]

e^x &= \sum_{n=0}^\infty \frac{x^n}{n!} \\[1em]

\arctan(x) &= \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{2n+1}, & |x| \leq 1 \\[1em]

\sin(x) &= \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!} \\[1em]

\cos(x) &= \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!}
\end{aligned}
$$
We can do u-substitutions here to replace the $x$ with whatever desired variable we want. 