This is essentially taking the [[Secant Lines]] of the function and then taking the [[Limit]] as the two points of the function approach each other. As the two points get infinitely close, the [[Secant Lines]] turn into a [[Tangent Line]].
With the function $f(x)$ at the point $x=a$, provided that the limit exists. 
## Newtons
$$
\begin{aligned}
f'(a)=\lim_{x\rightarrow a}\frac{f(x)-f(a)}{x-a}=\lim_{h\rightarrow 0}\frac{f(a+h)-f(a)}{h}
\end{aligned}
$$
>[!Note]
>The second form in this example takes the first point, $x,f(x)$ and then adds another point, $x+h,f(x+h)$. This indicates a infinitesimally small change.

## Leibniz
$$
\begin{aligned}
f'(a)&= \frac{df(x)}{dx}\Big|_{x=a}
\end{aligned}
$$ 
We can use the information above to see why the [[Derivative]] is the [[Slope]] of the function.
$$
\begin{aligned}
y&= mx+c\\
\lim_{x\rightarrow a}\frac{f(x)-f(a)}{x-a}&= \lim_{x\rightarrow a}\frac{(mx+b)-(ma+b)}{x-a}\\
&= \frac{mx-ma}{x-a}\\
&= m
\end{aligned}
$$
So for a linear function, this picks out the [[Slope]] of the line, this is because:
$$
\begin{aligned}
m=\frac{\Delta y}{\Delta x}=\frac{f(x)-f(a)}{x-a}
\end{aligned}
$$



