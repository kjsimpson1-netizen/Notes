In order for a [[System]] to be stable, we must have that the output signal, $|y(t)|<B,\forall{t}\in\mathbb{R}$ should always be bounded given a bounded input $|x(t)|<B,\forall{t}\in\mathbb{R}$. We can express this as the [[Math/10 - Signal Analysis/Convolution|Convolution]] of the input [[Signal]] and the [[Unit Impulse]] response, and if this is bounded, then the [[System]] is stable. 
$$
\begin{aligned}
|y|&= x*h\\
&=\int_{-\infty}^\infty |x(\tau)|h(t-\tau)d\tau\\
&\le B\int_{-\infty}^\infty h(t-\tau)d\tau
\end{aligned}
$$
Thus, the [[Integral]] of the impulse response must be bounded. 