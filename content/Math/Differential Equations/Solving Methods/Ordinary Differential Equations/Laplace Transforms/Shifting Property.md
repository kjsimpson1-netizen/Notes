## Frequency Shift
When we multiply one of the known [[Laplace Transforms]] by $e^{-at}$, we end up shifting it by $a$.
$$\begin{align*}
&\textcolor{red}{\bf{\text{Example 1}}}\\
\hline\\
F(s)&= 2\frac{2}{(s+1)^2+4}\\
\hline\\
u&= s+1\implies a=1\\
\hline\\
F(u)&= 2\frac{2}{u^2+2^2}\implies w=2\\
\hline\\
\mathcal{L}^{-1}&= \sin(wt)e^{-at}\\
&= \sin(2t)e^{-t}
\end{align*}$$
## Time Shift
This is for taking a given [[Laplace Transforms]] and translating it horizontally. We do this whenever we spot a $e^{as}$ in the [[Ordinary Differential Equations|ODE]], and this gives us the hint the the [[Laplace Transforms]] has been translated horizontally. 
$$\begin{align*}
&\textcolor{red}{\text{Example 2}}\\
\hline\\
&\mathcal{L}^{-1}\left\{\frac{e^{2s}}{s^2}\right\}\\
\hline\\
\mathcal{L}^{-1}&= u(t-a)f(t)\\
a=2&\quad f(t)=t\\
\hline\\
\implies\mathcal {L}^{-1}&= u(t-2)(t-2)
\end{align*}$$
