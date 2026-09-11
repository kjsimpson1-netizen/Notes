---
aliases:
  - Double Integral
---
 These are [[Integral|Integrals]] that have two different dimensions that are being taken into account rather than just one. If the physical interpretation of an integral is a area, then this would be a volume (provided it isn't [[Signed Area]], then this loses  it's physical interpretation). This is represented using the symbol:
$
\begin{aligned}
\iint_{\mathcal{R}} f(x,y)dx\;dy= \int dy\int dx\;f(x,y)=\iint_{\mathcal{R}}f(d,x)dA\\
\hline\\
\mathcal{R}=\{(x,y):g_1(y)\le x\le g_2(y),a\le y\le b\}
\end{aligned}
$
The equivalence above is an example of [[Fubini's Theorem]], as we can rewrite it as a [[iterated integral]] as well. 
>[!Note]
>The order of operations in which we have to take the integrals is from the inside most integrand outward. For each respective [[integral]] of a multivariable function, we treat the thing that we aren't integrating with respect to as a constant  (reminiscent of [[Partial Derivatives]]).

 