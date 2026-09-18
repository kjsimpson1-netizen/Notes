This is the most general form of the solution for [[Partial Differential Equations]]. These will take the form:
$$
\begin{aligned}
L\Big[\phi\Big]\equiv[p(x)\phi']'+q(x)\phi&= -\lambda w(x)\phi
\end{aligned}
$$
Where $\phi(x)$ are the [[Eigenfunction|Eigenfunctions]] and $\lambda$ are the [[Eigenvalues]]. This is valid on the domain from $x\in(0,l)$. It has the boundary conditions (also known as <u> seperated boundary conditions</u>):
$$
\begin{aligned}
\begin{cases}
\phi'(0)-h_1\phi(0)=0\\
\phi'(l)-h_\phi(l)=0
\end{cases}
\end{aligned}
$$
Assume for regular [[Sturm-Liouville]] that:
$$
\begin{aligned}
\begin{cases}
p(x)>0&&x\in[0,l]\\
w(x)>0&&x\in[0,l]\\
p,q,w,h,h_1\in\mathbb{R}
\end{cases}
\end{aligned}
$$
>[!Note]
>$w(x)$ is called the "weight function"

[[Separation of Variables]] is a special case of [[Sturm-Liouville]]
## Properties
We have that for all [[Sturm-Liouville]] problems, that:
### Eigenvalues
1. The [[Eigenvalues]] are real and non negative
2. $\lambda_1<\lambda_2<\lambda_3<...\lambda_i$
### Eigenfunctions
1. If $\lambda_i\neq\lambda_j$, then the two eigenfunctions are orthogonal
2. Any eigenfunction can be normalized
3. Completeness of eigenfunctions $\Phi_j(x),j\ge1$, in the sense that any $f(x)$ which is square integrable, can be expanded as $f(x)=\sum_{j=1}^\infty c_j\Phi_j(x)$ with "mean square convergence" at least.
>[!Note]
>In order to find $c_j$,  we can take:
>$$
\begin{aligned}
c_j&= \frac{\int_0^lf(x)w(x)\Phi_j(x)dx}{\int_0^lw(x)(\Phi_j(x))^2dx}
\end{aligned}
$$
## Regular Singular Points
If on the end of the domain of the differential equation, there is a regular singular point, we can evaluate it as before, however using a <u>soft boundary condtion</u> at the side with the singular point.
### Soft Boundary Condition
This is a boundary condition such that the boundary term vanishes at $x=0$. A sufficient condition  is that $\phi$ and $\phi'$ are <u>bounded</u> as $x$ goes to the singular point. This is so that:
$$
\begin{aligned}
\lim_{x\to0^+}p(x)\phi(x)=0&&\lim_{x\to0^+}p(x)\phi'(x)=0
\end{aligned}
$$
We first use [[Frobenius Method]] to solve for the [[Boundary Conditions]], then from there we use the fact that the [[Boundary Conditions]] must be bounded to choose them. 