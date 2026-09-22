The convolution sum uses the properties of an [[Linear Time Invariant System|LTI System]] system to show how a [[System]] will respond to any [[Signal]]. Using the [[Unit Impluse]] of a discrete system:
$$
\begin{aligned}
x[n]=\sum_{i=-\infty}^\infty x[i]\delta[n-i]
\end{aligned}
$$
We can state that if a [[System]] takes in a [[Unit Impluse]] and outputs $h$, that we can express this as:
$$
\begin{aligned}
\mathcal{L}\{\delta (t)\}= h(t)
\end{aligned}
$$
This means that we can write the output for any [[system]] as:
$$
\begin{aligned}
y(t)=\mathcal{L}\{x(t)\}=\sum_{i=-\infty}^\infty x(i)\cdot h(n-i)
\end{aligned}
$$
More formally, we can say that we are <u>convolving</u> the [[Signal]] $x$ and $h$:
$$
\begin{aligned}
y(t)=x(t)*h(t)
\end{aligned}
$$
