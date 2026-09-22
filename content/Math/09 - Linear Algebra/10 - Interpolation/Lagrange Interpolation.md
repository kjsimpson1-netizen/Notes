Given $N$ data points $(x_i,f(x_i))$, $i=1,\ldots,N$, there exists a **unique polynomial of degree $N-1$** that interpolates the data.
The Lagrange interpolating polynomial is
$$I(x)=\sum_{i=1}^{N}f(x_i)L_i(x)$$
where the **Lagrange basis (reference shape) functions** are
$$L_i(x)=\prod_{\substack{j=1\\j\neq i}}^{N}\frac{x-x_j}{x_i-x_j}.$$
These basis functions satisfy
$$L_i(x_j)=\begin{cases}1, & i=j,\\0, & i\neq j.\end{cases}$$
Therefore,
$$I(x_i)=f(x_i),$$
so the interpolating polynomial exactly matches the given data points.
### Interpolation Error
For a sufficiently smooth function $f$, the interpolation error can be expressed as
$$f(y)-I(y)=\frac{1}{3!}y(y^2-1)\frac{d^3f}{dy^3}(\zeta),$$
for some $\zeta$ in the interpolation interval.
If
$$\left|\frac{d^3f}{dy^3}\right|\leq K_3,$$
then
$$|f(y)-I(y)|\leq\frac{1}{6}\frac{2}{3\sqrt{3}}\left(\frac{h}{2}\right)^3K_3.$$
Thus,
$$|f(y)-I(y)|=\mathcal{O}(h^3).$$
Hence, this interpolation strategy is **third-order accurate**.