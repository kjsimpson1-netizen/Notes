This is a method for approximating any [[Definite Integral]]. This is particularly useful when the the integrals cannot be integrated analytically. This is more accurate than the trapezoidal approximation or [[Riemann Summations]].
$$
\begin{aligned}
\int_a^bf(x)dx&\approx \Delta x\cdot\frac13(f(a)+4f(x_1)+2f(x_2)...f(b))
\end{aligned}
$$
Where $\Delta x$ is the same as calculated for [[Riemann Summations]].
>[!Note]
>The number of terms must be even
## Error Bounds
The error of Simpson's rule can be found using:
$$
\begin{aligned}
\text{Error}(S_{N}) &\le  \frac{M (b-a)^5}{180 N^4}\\
\hline\\
b&= \text{Upper Bound}\\
a&= \text{Lower Bound}
\end{aligned}
$$
>[!Note]
>The value for $M$ here is the greatest absolute value for the fourth derivative of the function on the [[Interval]]. 


