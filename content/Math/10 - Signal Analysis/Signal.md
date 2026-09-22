A signal is any object that holds data, whether that be spatial coordinates, color attributes of a pixel, and anything else. A signal breaks into a few subcategories:
## Continuous Signals
These are signals that aren't quantized, and rather persist. No matter how much you subdivide the time, these will still be continuous. They are represented by round brackets, $x(t)$ 
## Discrete Signals
These are signals that are broken into discrete quanta. They are represented by square brackets, $x[n]$. We can represent these by a sum of Delta functions:
$$
\begin{aligned}
x[n]=\sum_{i=-\infty}^\infty x[i]\delta[n-i]
\end{aligned}
$$
