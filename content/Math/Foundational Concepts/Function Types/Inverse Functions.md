These are any function that has it's output equivalent to the input of the original function. The notation of these can take multiple forms, either:
$$
$$\begin{aligned}
f^{-1}(x)\text{ or }f(y)
\end{aligned}$$
$$
with $f(x)$ being the original function. Another defining characteristic of these is that they are mirror from the original function over the line $y=x$. We can do this because it has the effect of swapping the x values and the y values.
```desmos-graph
y=x | dotted
e^x
\log(x)
```
## Exceptions
### Radicals
Because these are still a type of function, they must still pass the vertical line test. This means for certain graphs, such as quadratics and [[Trigonometric Functions]], they will fail the vertical line test:
For example, if we just reflect $x^2$:
```desmos-graph
y=x^2
y=x |dotted
y=\sqrt{x} |green
y=-\sqrt{x} | green
```
There are too many values for each x input value here. We can fix this by restricting the domain of $x^2$ to where it is increasing, therefore when it is greater than 0
```desmos-graph
x^2
\sqrt{x}
x | dotted
```
### $\sin(x)$
We have the same issue here, with each y value corresponding to infinitely many x values. Therefore we must limit it's domain
```desmos-graph
\sin(x)
```
We can therefore represent this as an inverse, or arcsine:
```desmos-graph
top = 2; bottom = -2;
left = -1.5; right = 1.5;
---
\arcsin(x)
```
### $\cos(x)$
The same deal goes for cosine:
```desmos-graph
top = 4; bottom = 0;
left = -1.5; right = 1.5;
---
\arccos(x)
```
