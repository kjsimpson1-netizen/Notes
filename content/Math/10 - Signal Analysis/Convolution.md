The convolution uses the properties of an [[Linear Time Invariant System|LTI System]] system to show how a [[System]] will respond to any [[Signal]]. We can think of this as dragging a [[unit impulse]] over the entire [[Signal]] to see how the [[System]] reacts. 
## Discrete Time
Using the [[Unit Impulse]] of a discrete system:
$$
\begin{aligned}
x[n]=\sum_{i=-\infty}^\infty x[i]\delta[n-i]
\end{aligned}
$$
We can state that if a [[System]] takes in a [[Unit Impulse]] and outputs $h$, that we can express this as:
$$
\begin{aligned}
\mathcal{L}\{\delta [n]\}= h[n]
\end{aligned}
$$
This means that we can write the output for any [[system]] as:
$$
\begin{aligned}
y[n]=\mathcal{L}\{x[n]\}=\sum_{i=-\infty}^\infty x[i]\cdot h[n-i]
\end{aligned}
$$
More formally, we can say that we are <u>convolving</u> the [[Signal]] $x$ and $h$:
$$
\begin{aligned}
y[n]=x[n]*h[n]
\end{aligned}
$$
## Continuous Time
Using the [[Unit Impulse]] of a continuous system:
$$
\begin{aligned}
x(t)=\int_{-\infty}^\infty x(\tau)\delta(t-\tau)\,d\tau
\end{aligned}
$$
We can state that if a [[System]] takes in a [[Unit Impulse]] and outputs $h$, that we can express this as:
$$
\begin{aligned}
\mathcal{L}\{\delta (t)\}= h(t)
\end{aligned}
$$
This means that we can write the output for any [[system]] as:
$$
\begin{aligned}
y(t)=\mathcal{L}\{x(t)\}=\int_{-\infty}^\infty x(\tau)\cdot h(t-\tau)\,d\tau
\end{aligned}
$$
More formally, we can say that we are <u>convolving</u> the [[Signal]] $x$ and $h$:
$$
\begin{aligned}
y(t)=x(t)*h(t)
\end{aligned}
$$