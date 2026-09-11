This is a form of [[Riemann Summations]] to approximate the area of a [[Definite Integral]]:
This is when the average of the RRAM and the LRAM is taken. This is generally the most accurate for estimating the area under a function
$$
$$
\begin{aligned}
\text{Trapezoid Approximation}&= \frac12(\text{RRAM+LRAM})
\end{aligned}
$$
$$
![[Trapezoid Approx.png]]
$$
$$
\begin{aligned}
\int_a^bf(x)dx&\approx \left(\frac{b-a}{2n}\right)\left(f(a)+2\sum_{i=1}^{n-1}f\left(a+i\cdot\frac{b-a}{n}\right)+f(b)\right)\\
\hline\\
a&= \text{Lower Bound}\\
b&= \text{Upper Bound}\\
n&= \text{Steps}\\
f(x)&= \text{Function}
\end{aligned}
$$
$$
## Error Bound
The maximum error that this can have on a given [[Interval]] is given by:
$$
$$
\begin{aligned}
\text{Error}(T_{N}) &\le  \frac{M(b - a)^3}{12N^2}\\
\hline\\
b&= \text{Upper Bound}\\
a&= \text{Lower Bound}
\end{aligned}
$$
$$
>[!Note]
>The value for $M$ here is the greatest value for the second derivative of the function on the interval. This can be found using the [[Second Derivative Tests]].

