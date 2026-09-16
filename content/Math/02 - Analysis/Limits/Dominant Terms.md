When there are two competing factors, either a numerator and a denominator or even two functions, then we can use the concepts from [[Comparing Functions]] to determine which one will dominate.
## Rationales
$$
\begin{aligned}
\lim_{x\rightarrow\infty}\frac {x^3} {x^7}&= 0\\
\lim_{x\rightarrow\infty}\frac1x&= 0\\
\lim_{x\rightarrow\infty}\frac{7x^3+8x+10}{2x^3+4x+10}&\approx \frac{7x^3}{2x^3}\\
&= \frac72
\end{aligned}
$$For these ones, whichever one has a much higher degree will dominate and therefore the value of $f(x)$ will approach whichever the dominant term leans towards.
## Exponentials
$$
\begin{aligned}
\lim_{x\rightarrow \infty}e^x&= +\infty\\
\lim_{x\rightarrow-\infty}e^x&= 0
\end{aligned}
$$
Because exponentials have two very distinct ends, one of them will always approach [[Infinity]] while the other will always approach 0.
```desmos-graph
y=e^x
```
$$
\begin{aligned}
\lim_{x\rightarrow\infty}\frac{x^2}{e^x}&= 0\\
\lim_{x\rightarrow-\infty}\frac{x^2}{e^x}&= +\infty\\
\end{aligned}
$$
## Trigonometry
$$
\begin{aligned}
\lim_{x\rightarrow \infty}\sin (x)&= \text{DNE}\\
\lim_{x\rightarrow \infty}\cos (x)&= \text{DNE}\\
\lim_{x\rightarrow \infty}\tan (x)&= \text{DNE}
\end{aligned}
$$
All three of the trigonometric functions do not have a limit as x approaches [[Infinity]] because they constantly oscillate and never actually approach a single number as a [[Limit]]. However, for $\sin$ and $\cos$, if they are a part of a a function in which they are multiplied by another term, we can use the [[Sandwich Theorem]] to determine the value at a certain point. 

