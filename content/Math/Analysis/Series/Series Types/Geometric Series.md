These are [[Math/Analysis/Series/Series]] where each following term is a constant multiple of the previous term, and we can represent this as:
$
$
\begin{aligned}
\sum_{n=0}^\infty ar^n
\end{aligned}
$
$
With $a$ being the starting value and the ratio being represented as:
$
$
\begin{aligned}
r&= \frac{a_{n+1}}{a_n}
\end{aligned}
$
$
(Note that this looks very similar to the [[Ratio Test]])
## Infinite Geometric Series
We can calculate the sum of the [[Sequences]] by doing the following:
$
$
\begin{aligned}
S_\infty&= \frac a{1-r}
\end{aligned}
$
$
Where $a=a_0$ and $r$ is the ratio of subsequent terms. 
## Closed Interval
If the series takes place on a finite interval, the [[Math/Analysis/Series/Series]] can be calculated by:
$
$
\begin{aligned}
S_n&= a\frac{1-r^{n+1}}{1-r}
\end{aligned}
$
$
>[!Note]
>This can be used to find the decimal expression for repeated decimals. For example, $0.\bar{33}$ can be rewritten as:
>$
$
\begin{aligned}
0.\bar{33}=\sum_{n=0}^\infty\frac3{10}\cdot\left(\frac1{10}\right)^n
\end{aligned}
$
$
Then using the expression for infinite geometric series:$
$
\begin{aligned}
\sum_{n=0}^\infty\frac3{10}\cdot\left(\frac1{10}\right)^n&= \frac a{1-r}\\
&= \frac{\frac3{10}}{1-\frac1{10}}\\
&= \frac3{10-1}\\
&= \frac13
\end{aligned}
$
$
This is then the exact fraction representation of the repeated decimal

