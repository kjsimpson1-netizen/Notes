## Lagrange Interpolation
Given Lagrange Interpolating Polynomials, and $N$ $f(x_i),i\le N$, Then there is a unique degree $N-1$ polynomial that fits this data. This is expressed by:
$$
\begin{aligned}
I(x)=\sum_{i=1}^Nf(x_i)\cdot\underbrace{\frac{\prod_{j\neq 1}(x-x_j)}{\prod_{j\neq 1}(x_i-x_j)}}_{\text{Reference shape functions}}
\end{aligned}
$$
>[!Note]
>There is a theorem that states that if:>$$
\begin{aligned}
f(y)-S(y)=\frac16y(y^2-1)\frac{d^3f}{dy^3}f(\zeta)
\end{aligned}
$$
Then:$$
\begin{aligned}
|f(y)-S(y)|&\le \frac16\cdot\frac2{3\sqrt{3}}\left(\frac h2\right)^3K_3
\end{aligned}
$$
This means that it is a third order accurate strategy. 

## Cubic Hermite Interpolation

## Fourier Functions
These functions are defined by $f(x)=\frac1{2\pi}\exp(i\alpha x),\alpha\in\mathbb{Z}$, where $f(x)$ are [[Eigenfunction|Eigenfunctions]] and they form an [[Eigenbasis]]. We can then take these as an infinite series to form:
$$
\begin{aligned}
g(x)=\frac1{\sqrt{2\pi}}\sum_{\alpha=-\infty}^{\infty}\hat g_\alpha e^{i\alpha x}
\end{aligned}
$$
Where $\hat g_\alpha$ are the coefficients, defined by:$$
\begin{aligned}
\hat g_\alpha =\frac1{\sqrt{2\pi}}\int_0^{2\pi}g(x)e^{-i\alpha x}
\end{aligned}
$$This infinite sum can be used to represent any given function. We have that:$$
\begin{aligned}
|\hat g_\alpha|\le\frac{k_m}{|\alpha|^{m-2}}\qquad K_m\equiv ||g^{(m)}||_\infty
\end{aligned}
$$
## Spectral Interpolation
This is given by a finite series of Fourier functions:$$
\begin{aligned}
G_M=\sum_{-M}^M\hat g_\alpha e^{i\alpha x}
\end{aligned}
$$The [[Maximum Norm]] of this interpolant is:
$$
\begin{aligned}
||G_M-f)||_\infty&\le CK_m\cdot M^{2-m}
\end{aligned}
$$
This is defined as <u>spectral convergence</u>.
## Discretized Version
If we have a grid of $N=2M$, with $x_j=\frac{2\pi j}N, j\in[1,N]$, and:
$$
\begin{aligned}
F_j&= f(x_j)\\
&= \sum_{\alpha=-\infty}^\infty\hat f_\alpha e^{i\alpha x_j}\\
&= \sum_{\alpha=-\infty}^\infty\hat f_\alpha e^{\frac{2\pi\alpha}Ni}\\
&= \underbrace{\sum_{\alpha=0}^{N-1}e^{\frac{2\pi\alpha}Ni}}_{\text{Fourier Vectors}}\underbrace{\sum_{l=-\infty}^\infty\Big(\hat f_\alpha +lN\Big)}_{\text{DF Coefficients}}
\end{aligned}
$$
>[!Note]
>Aliasing is when high frequency components of $f$ are see as low frequency of the grid. 

We can then define:$$
\begin{aligned}
D_\alpha\equiv e^{\frac{2\pi\alpha}Ni}
\end{aligned}
$$These values are all [[Orthogonal]]. Thus:$$
\begin{aligned}
F=\sum_{\alpha=0}^{N-1}\hat F_\alpha D_\alpha
\end{aligned}
$$We can then take the [[Inner Product]] of the following to get the coefficients:
$$
\begin{aligned}
\braket{F,D_\alpha}=N\hat F_{\alpha}
\end{aligned}
$$This can also be done very quickly with a Fast Fourier Transform.