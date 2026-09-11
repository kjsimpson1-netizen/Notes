To find the horizontal asymptotes, take the dominant terms (highest degree) of the numerator and the denominator and the quotient of the two is the horizontal asymptote. However, if the degree of the two leading terms do not match, then the larger one will decide what the graph will do. 
If the numerator has a larger degree, then the graph will have a horizontal asymptote at $x=0$, but if the denominator has the higher degree, then the horizontal asymptote will not exist. 
```desmos-graph
y=1/x+2
y=2 |red|dashed
```
## Limits
We can also use the [[Limit]] to see this more clearly. If $\lim_{x\rightarrow\infty}f(x)=L$ or $\lim_{x\rightarrow-\infty}f(x)=-L$
then $y=L$ is a horizontal asymptote. (only if the value is a finite number). We can see that this is true because as the x-values approach [[Infinity]] in either direction, the approach, but never touch the horizontal asymptote, which is exactly what a [[Limit]] does. 
Some special cases of this are when the function has a trigonometry term multiplied by it, as this will cause the function to oscillate. We can use the [[Sandwich Theorem]] here to solve for the value that it will approach, as it never approaches one defined value if it oscillates. 
