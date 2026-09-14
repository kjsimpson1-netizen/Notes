We can use substitution to turn one two variable problem into another in the form of [[Polar Coordinates]]. This can be done by:
1. Rewriting $x$ and $y$ and $r\cos\theta$ and $r\sin\theta$ respectively
2. Setting the limits ($r$ is the distance from the origin, and $\theta$ is the angular span) 
3. Plug into the form:$$
\begin{aligned}
\iint_{\mathcal{R}}f(x,y)dA=\iint r\cdot f(r\cos\theta,r\sin\theta)dr\;d\theta
\end{aligned}
$$
>[!Note]
>The radius integration is usually done first, and the formula includes the extra $r$ to account for polar stretching

These questions often include a product of terms with $r$ and other terms with $\theta$, which means that we can often rewrite this as a [[Iterated Integral]].