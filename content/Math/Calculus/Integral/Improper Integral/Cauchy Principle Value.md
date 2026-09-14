This method, often abbreviated to *P.V.*, is used to evaluate [[Improper Integral]]. This is used when a function has a loss of [[Continuity]], either at the [[Bounds]] or in the [[Interval]], of the [[Integral]]. We can still evaluate this by making the bounds into a [[Limit]]:
>[!Note]
>The bound that is taken as a [[Limit]] is the one that is not evaluable with the given value of the function
$$
\begin{aligned}
\int_a^bf(x)dx&= \lim_{t\rightarrow a^+}\int_t^bf(x)dx
\end{aligned}
$$

And if this function has a discontinuity somewhere where $c\in[a,b]$, then we can break it up into two different integrals. However, if either of the pieces doesn't exist, then the overall [[Integral]] doesn't exist. 
>[!Warning]
>If this does not approach a single value, then the [[Improper Integral]] is considered to be divergent

