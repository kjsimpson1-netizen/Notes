These are any circuit that contain an [[Inductor]] and a [[Resistor]]. The inductor's job is to counteract the change that occurs in the current. The time constant for a R-L circuit, with the time constant being what percentage of the final current value that the [[Current]] has obtained, and is expressed by:
$$\begin{align*}
\tau&= \frac LR\\
\hline\\
\tau&= \text{Time Constant}\\
L&= \text{Inductance}\\
R&= \text{Resistance}
\end{align*}$$
## Current
The [[Current]] of an RL circuit can be expressed by the following:
$$\begin{align*}
i(t)&= \frac {\mathcal{E}}R\left(1-e^{-\frac RLt}\right)\\
\hline\\
i(t)&= \text{Current}\\
\mathcal{E}&= \text{Voltage}\\
R&= \text{Resistance}\\
L&= \text{Inductance}\\
t&= \text{Time}
\end{align*}$$
We can then also take the derivative of this to express the rate at which the current through the [[Inductor]] changing:
$$\begin{align*}
\frac{di(t)}{dt}&= \frac {\mathcal{E}}Le^{-\frac RLt}\\
\hline\\
i(t)&= \text{Current}\\
\mathcal{E}&= \text{Voltage}\\
R&= \text{Resistance}\\
L&= \text{Inductance}\\
t&= \text{Time}
\end{align*}$$
## Inductor as a current source
If the inductor becomes the current source of the circuit, the expression for the current flowing through it is:
$$\begin{align*}
I(t)&= I_0e^{-\frac t\tau}\\
\hline\\
I&= \text{Current}\\
t&= \text{Time}\\
\tau&= \text{Time Constant}
\end{align*}$$
