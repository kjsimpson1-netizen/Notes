This is a method to find the roots of a function that are not easily factorable. This is done using the [[Tangent Line]] of a function at a point, $x_0$, that is a close guess to the root that you're trying to find. You can then use the root of that [[Tangent Line]], $x_0$, as the next guess for the method. This will allow the root to be found much quicker than using halving methods. The equation for find the next root of the Newton-Raphson is:
$
$
\begin{aligned}
x_{n+1}&= x_n-\frac{f(x_n)}{f'(x_n)}
\end{aligned}
$
$
## Example
```desmos-graph
f(x)=(x-1)^2-1
g(x)=(-4)x-1
(-1/4,0)
```
```desmos-graph
f(x)=(x-1)^2-1
g(x)=-2.5x-0.0625
(-0.025,0)
```
And this will keep moving towards the root
## Error

For this method, we have that $x_{n+1}=x_n-g(x_n)$, where $g(x)=\frac{f(x)}{f'(x)}$. We will then get a quadratic approximation of $g(x)$ based on $x=x_*$.

$
$
\begin{aligned} 
g(x)&\approx \cancel{g(x_*)}+g'(x_*)(x-x^*)+\frac12g''(x_*)(x-x_*)^2\\
g'(x)&= 1-\frac{f(x)f''(x)}{\Big(f(x)'\Big)^2}\\
g''(x)&= -\frac{f''(x_*)}{f'(x_*)} 
\end{aligned}
$
$

Since $f(x_*)=0$, we have $g(x_*)=0$ and $g'(x_*)=1$. Therefore,

$
$
\begin{aligned} 
g(x)&\approx (x-x_*)-\frac{f''(x_*)}{2f'(x_*)}(x-x_*)^2 
\end{aligned}
$
$

Plugging this in gives us:

$
$
\begin{aligned} 
g(x_n)&= \underbrace{(x_n-x_*)}_{e_n}-\underbrace{c(x_n-x_*)^2}_{e_n^2}\\
c&=\frac{f''(x_*)}{2f'(x_*)} 
\end{aligned}
$
$

Which gives:

$
$
\begin{aligned} 
x_{n+1}:&= x_n-g(x_n)\approx x_n-\left[(x_n-x_*)-c(x_n-x_*)^2\right]\\
&=x_*+c(x_n-x_*)^2
\end{aligned}
$
$

This leads us to:

$
$
\begin{aligned} 
e_{n+1}&=x_{n+1}-x_*\\
&\approx c(x_n-x_*)^2\\
&=ce_n^2
\end{aligned}
$
$