## Integrals
This is another test to see if the [[Improper Integral]] due to a [[Singular Point]] using the [[Cauchy Principle Value]] will converge or diverge. The general rule for this is that for any function with [[Continuity]], with $a=-\infty$ and/or $b=+\infty$, and letting the following being true:
$$
\begin{aligned}
F=\int_a^bf(x)dx\qquad G=\int_a^bg(x)dx
\end{aligned}
$$
>[!Note]
>The function $g$ here is the [[Comparison Function]]
## 1. 
If $|f|\in[0,|g|]$ for all $x\in(a,b)$ and if $G$ converges, then $F$ also converges with $F<G$
## 2.
If $|f|\in[|g|,\infty]$ for all $x\in(a,b)$ and if $G$ diverges, then $F$ also diverges
## Series
This works the exact same way as with integrals, however with series. However, to find the [[Comparison Function]], we may need to introduce another function with a constant $K$, so that the direct comparison test holds true and we can still compare the asymptotic behavior as $n\rightarrow\infty$. We can also compare a [[Math/Analysis/Series/Series]] to an [[Integral]], such as comparing the harmonic series ($\frac1n$) to the [[P-Series Test]] for $p=1$.