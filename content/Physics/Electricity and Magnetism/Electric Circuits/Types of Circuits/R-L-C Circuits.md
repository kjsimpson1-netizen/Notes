These are circuits that have [[Inductor]], [[Resistor]] and [[Capacitor]]. These act much the same as [[L-C Circuits]] with the oscillation of the [[Current]], however the [[Resistor]] will cause a dissipation of the energy and the current in the circuit, causing an exponential decay.
```desmos-graph
y=e^{-0.2(x+5)}*5\sin(4/(\pi) (x+5))
```
## Charge
The equation of the charge of this is:
$$
\begin{aligned}
q(t)&= Ae^{-\frac t\tau}\cos(\omega't+\phi)\\
\hline\\
q&= \text{Charge}\\
A&= \text{Initial Value}\\
t&= \text{Time}\\
\tau&= \text{Time Constant}\\
\omega&= \text{Frequency}\\
\phi&= \text{Phase Angle}
\end{aligned}
$$
## Time Constant
The time constant of an L-R-C circuit is:
$$
\begin{aligned}
\tau&= \frac{2L}R\\
\hline\\
\tau&= \text{Time Constant}\\
L&= \text{Inductance}\\
R&= \text{Resistance}
\end{aligned}
$$
## Frequency
The angular frequency of these oscillations can be expressed by the following:
$$
\begin{aligned}
\omega'&= \sqrt{\frac1{LC}-\frac{R^2}{4L^2}}\\
\hline\\
\omega&= \text{Angular Frequency}\\
L&= \text{Inductance}\\
C&= \text{Capacitance}
\end{aligned}
$$
## Potential Energy
The potential energy of this system is given by the summation of the potential energy of the [[Capacitor]] and the potential energy of the [[Inductor]]:
$$
\begin{aligned}
U&= \frac{q^2}{2C}+\frac{Li^2}{2}\\
\hline\\
U&= \text{Potential Energy}\\
q&= \text{Charge}\\
C&= \text{Capacitance}\\
L&= \text{Inductance}\\
i&= \text{Current}
\end{aligned}
$$
# With a Power Supply
If there is a power supply attached, the total magnitude of the voltage can be expressed by a relation of the [[Voltage]] to the [[Current]] and the total [[Impedance]] with.
$$
\begin{aligned}
V&= IZ\\
\hline\\
V&= \text{Voltage Amplitude}\\
I&= \text{Current Amplitude}\\
Z&= \text{Impedance}
\end{aligned}
$$
>[!Note]
>When there is a parallel LRC circuit:
>1. Voltage: The phase shifted voltage can be added up with respect to the common current
>2. Current: The phase shifted current can be added up with respect to the source voltage
