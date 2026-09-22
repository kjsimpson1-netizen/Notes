## Fourier Functions
The **Fourier basis functions** are defined by
$$f_\alpha(x)=\frac{1}{\sqrt{2\pi}}e^{i\alpha x},\qquad\alpha\in\mathbb{Z}.$$
These functions are [[Eigenfunction|eigenfunctions]] and form an [[Eigenbasis]] for periodic functions on $[0,2\pi]$.

We can represent a function $g(x)$ as an infinite Fourier series:
$$g(x)=\frac{1}{\sqrt{2\pi}}\sum_{\alpha=-\infty}^{\infty}\hat g_\alpha e^{i\alpha x},$$
where $\hat g_\alpha$ are the Fourier coefficients, given by
$$\hat g_\alpha=\frac{1}{\sqrt{2\pi}}\int_0^{2\pi}g(x)e^{-i\alpha x}\,dx.$$
For a sufficiently smooth function, the Fourier coefficients decay according to
$$|\hat g_\alpha|\leq\frac{K_m}{|\alpha|^m},\qquad K_m\equiv\left\|g^{(m)}\right\|_\infty.$$
Thus, smoother functions have faster-decaying Fourier coefficients.

## Spectral Interpolation
A finite Fourier series can be used to approximate $g(x)$:
$$G_M(x)=\frac{1}{\sqrt{2\pi}}\sum_{\alpha=-M}^{M}\hat g_\alpha e^{i\alpha x}.$$
The [[Maximum Norm]] of the interpolation error satisfies
$$\left\|G_M-g\right\|_\infty\leq C K_m M^{2-m},$$
for some constant $C$.

This rapid convergence for sufficiently smooth functions is called **spectral convergence**.

## Discretized Version
Consider a grid of $N=2M$ points,
$$x_j=\frac{2\pi j}{N},\qquad j=0,\ldots,N-1.$$
Evaluating the Fourier series at the grid points gives
$$F_j=g(x_j)=\sum_{\alpha=-\infty}^{\infty}\hat g_\alpha e^{i\alpha x_j}.$$
Since
$$x_j=\frac{2\pi j}{N},$$
we have
$$F_j=\sum_{\alpha=-\infty}^{\infty}\hat g_\alpha e^{2\pi i\alpha j/N}.$$
Because
$$e^{2\pi i(\alpha+lN)j/N}=e^{2\pi i\alpha j/N},$$
frequencies that differ by multiples of $N$ are indistinguishable on the discrete grid. Therefore, the discrete Fourier coefficients are
$$\hat F_\alpha=\sum_{l=-\infty}^{\infty}\hat g_{\alpha+lN}.$$
These are the **DFT coefficients**.

> [!NOTE]
> **Aliasing** occurs when high-frequency components of $g$ are represented as lower-frequency components on the discrete grid.

We can define the discrete Fourier vectors as
$$D_\alpha(j)\equiv e^{2\pi i\alpha j/N},\qquad\alpha=0,\ldots,N-1.$$
These vectors are [[Orthogonal]], satisfying
$$\langle D_\alpha,D_\beta\rangle=N\delta_{\alpha\beta}.$$
Therefore, the discrete function can be written as
$$F=\sum_{\alpha=0}^{N-1}\hat F_\alpha D_\alpha.$$
Taking the [[Inner Product]] with $D_\alpha$ gives the coefficients:
$$\langle F,D_\alpha\rangle=N\hat F_\alpha,$$
and hence
$$\boxed{\hat F_\alpha=\frac{1}{N}\langle F,D_\alpha\rangle}.$$
These coefficients can be computed efficiently using the **Fast Fourier Transform (FFT)**.