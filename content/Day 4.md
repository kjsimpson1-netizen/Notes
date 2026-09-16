## Interpolation
This is the idea of matching a function to a set of points. Given an interval $x\in[a,b]$ with $N$ sub divisions, each with width $h=\frac{b-a}N$. On each subinterval, the function will be approximated using a polynomial to give a global approximation of $f(x)$.
### Convergence
If the magnitude of the [[Operator Norm]] approaches 0, or $\lim_{N\to\infty}||F_N(x) - f(x)||_\infty=0$, then the interpolation strategy converges.
### Order of Convergence
If $||F_N(x) - f(x)||_\infty\le Ch^p\quad p>0$, then we can say that it converges with order $p$.

### Linear Approximation
On the subinterval with center point$x_j$, we will take a linear approximation of:
$$
\begin{aligned}
f(x)&\approx f(x_j)+\frac d{dx}f(x_j)(x-x_j)
\end{aligned}
$$
>[!Note]
>$$
\begin{aligned}
f(x)-L(x)=\underbrace{\frac{f''(\zeta)}2}_{\text{Error}}(x-x_j)^2
\end{aligned}
$$
At some point $\zeta\in(x_j-\frac h2,x_2+\frac h2)$ 
Define:$$
\begin{aligned}
\max_{x\in[a,b]}|f^{(n)}|:=K_n
\end{aligned}
$$Then we have that:$$
\begin{aligned}
|f(x)-L(x)|&\le k_2\frac{h^2}8\qquad||f-F_N||_\infty\le k_2\frac{h^2}8
\end{aligned}
$$
This just implies that the order of convergence is second order

The problem with this application is that the interpolated function will be discontinuous, and that you will need function values
## Linear Interpolation
This will use $N+1$ values at subinterval ends. On each subinterval, we will use [[Secant Lines]] approximations. 
## Rolle's Theorem
Let $f\in\mathcal{C}_1$ and $f(a)=f(b)=0$, then $\exists \zeta\in[a,b] \text{ s.t } f'(\zeta)=0$.
## Error Theorem
For any function approximated by [[Taylor Polynomials]], the error will be given by$$
\begin{aligned}
e_n=\frac{f^{(n+1)}(\zeta)}{(n+1)!}(x-a)^{n+1}
\end{aligned}
$$
