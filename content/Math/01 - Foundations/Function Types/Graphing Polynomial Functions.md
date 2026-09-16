#### Sketching $f(x)=x^2-x^4$
1. After some factoring, we can find the 3 x-intercepts:
$$
\begin{aligned}
f(x)&= x^2-x^4\\
&= x^2(1-x^2)\\
&= x^2(1-x)(1+x)
\end{aligned}
$$
We now have a graph that looks like this:
![[GraphingPolynomials1.png|600]]
2. Now, using the concepts that we learned in [[Comparing Functions]], we can infer what the graph will look like, almost thinking about it as a [[Piecewise Function]]:
$$
\begin{aligned}
f(x)\approx\begin{cases}
\text{When } x \text{ is large}, f(x)=x^2\\
\text{When }x\text{ is small}, f(x)=-x^4\\
\end{cases}
\end{aligned}
$$
This means that closer to 0, the graph $f(x)=x^2$ will be [[Dominant Terms]] and therefore the function will appear more similar to it, and the farther away from 0 the function is, the more like $f(x)=x^4$ the graph will appear, giving us the graph below:
![[GraphingPolynomials2.png|600]]
3. We can now put all these steps together, following the general shapes to make the graph have [[Continuity]].
![[GraphingPolynomials3.png|600]]
#### Sketching $f(x)=e^x-x^4$
1. We can't really find the x-intercepts easily for this one, so we can approximate
2. From comparing [[Dominant Terms]] of this function, we can see that:
   $$
\begin{aligned}
f(x)\approx\begin{cases}
\text{When } x \text{ is negative/small    }, f(x)=x^4\\
\text{When }x\text{ is postive and large}, f(x)=-e^x\\
\end{cases}
\end{aligned}
$$
From this, we can follow the steps from the previous example to arrive at these two graphs:
![[GraphingPolynomials4.png|600]]
We can now overlay the two graphs again, connecting them up to arrive at the following graph, noting that the more positive the variable, the more pull that the $e^x$ has on the graph:
![[GraphingPolynomials5.png|600]]


