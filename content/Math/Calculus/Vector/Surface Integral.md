---
aliases:
  - Flux Integral
---
This is very similar to taking a [[Line Integrals|Line Integral]], however now over a surface parameterized by two variables, not one. These exist in $\mathbb{R}^3$, however the surfaces themselves are a $\mathbb{R}^2$ element. An example of these are [[Magnetic Flux]] and [[Electric Flux]], or surface integrated with respect to a given [[Vector Field|Vector Fields]].  This takes the form:
$
$
\begin{aligned}
\iint_D f(x,y,z)dS=\iint_Df(\vec r(u,v)\underbrace{|\vec r_u\times \vec r_v|dudv}_{dS}=\iint_D\vec F\cdot d\vec S
\end{aligned}
$
$
We can think of this as the [[vector field]] being the velocity of a fluid flowing through a membrane (the surface). 
>[!Note]
>The order that we take of the [[Cross Product]] will decide whether or not the sign will be positive of negative. 