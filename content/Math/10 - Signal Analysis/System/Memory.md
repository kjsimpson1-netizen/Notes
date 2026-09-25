A [[system]] is said to have memory if if depends on a time other than the current time, $t_0$. Some examples of these are [[System|Systems]] that include [[Derivative|Derivatives]] or [[Integral|Integrals]], as these both depend on states other than the current values. Another example of a system with memory is one that refers to another point in time, i.e.:
$$
\begin{aligned}
y(t)=x(t-1)
\end{aligned}
$$
This is stating that the current state of [[Signal]] $y$ is dependent on a previous state of $x$. 
In order for a system to be memoryless, it's response to a [[Unit Impulse]] must be a scaled version of that [[Unit Impulse]]:
$$
\begin{aligned}
h(t)=\mathcal{L}\{\delta (t)\}=C\delta (t)
\end{aligned}
$$
