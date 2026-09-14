## Part 1
This theorem states that for any function, $f(t)$, with [[Continuity]], the following is true:
$$\begin{align*}
\frac{d}{dx}\int_{x_1}^{x_2}f(t)dt&= f(x_2)\cdot x_2'-f(x_1)\cdot x_1'
\end{align*}$$
Or less formally, the [[Integral]] (more formally an [[Antiderivative]]) of a [[Derivative]] is equal to the original function.
## Part 2
This is part that will allow us to take the [[Integral]] of any function where both of the bounds are non-zero:
$$\begin{align*}
\int_a^bf(x)dx&= \int_0^bf(x)dx-\int_0^af(x)dx
\end{align*}$$
This is true because the area from 0 to $a$ will cancel out the area from 0 to $b$. We can then evaluate this using the [[Antiderivative]] of the function to give us the following:
$$\begin{align*}
\boxed{\int_a^bf(x)dx=F(b)-F(a) }
\end{align*}$$
