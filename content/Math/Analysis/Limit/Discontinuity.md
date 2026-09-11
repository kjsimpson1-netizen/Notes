Discontinuity is when at least one of the [[One Sided Limits]] or the function evaluated at $x=a$ are not equivalent, and therefore the function at $x=a$ doesn't have [[Continuity]].
There are a few type of discontinuities depending on which part is unequal.
## Jump Discontinuities
These are discontinuities that have a [[Limit]] for both the top and bottom, but both [[One Sided Limits]] have different values. The function evaluated at this point exists at one side or the other, or neither but not both as this would break the vertical line test.
$$\begin{align*}
\lim_{x\rightarrow a^+}f(x)&\neq \lim_{x\rightarrow a^-}f(x)\\
&\text{but both exist}
\end{align*}$$
```desmos-graph
f(x)=1|x<1
g(x)=-1|x>1
```

## Infinite Discontinuities
This is when both [[One Sided Limits]] approach [[Infinity]], and these occur at a [[Singular Point]]
$$\begin{align*}
\lim_{x\rightarrow a^+}f(x)&= \pm\infty\\
\lim_{x\rightarrow a^-}f(x)&= \pm\infty
\end{align*}$$
```desmos-graph
1/x^2
```
## End-Point Discontinuities
This is when only 1 of the [[One Sided Limits]] exists
```desmos-graph
y=x^2|x<2
```
## Mixed Discontinuity
At least one of the two [[One Sided Limits]] do not exist
## Removable Discontinuities
These are discontinuities that can be removed by adding in another single point to "patch" a small hole in the graph without changing the overall graph. These are often caused by a portion of the numerator matching that of the denominator, causing a division of 0 by 0 at this point and appearing to equal [[Infinity]]. 

$$\begin{align*}
\lim_{x\rightarrow a}f(x)\text{ exists, but }f(a)\text{ doesn't}
\end{align*}$$
This can be repaired with the following [[Piecewise Function]]
$$\begin{align*}
f(x)=\begin{cases}
f(x)&,x\neq a\\
\lim_{x\rightarrow a}f(x)&, x=a\\
\end{cases}
\end{align*}$$
These can be patched by evaluating the function at the point that the discontinuity was removed from (the term that was factored out)
```desmos-graph
\frac{(x-1)x^2}{(x-1)}
(1,1)
```
