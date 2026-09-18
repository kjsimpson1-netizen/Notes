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