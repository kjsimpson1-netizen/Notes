These are circuits characterised by having a [[Capacitor]] and a [[Inductor]]. These circuits will creating an oscillating [[Current]] with the same magnitude. This happens because as the [[Capacitor]] discharges, the current increases at a decreasing rate. Therefore, the [[Current]] flowing through the [[Inductor]] will be changing, and the inductor will create a back EMF to oppose it. Overall, the energy in the circuit changes between the electrical energy of the capacitor and the magnetic energy of the inductor. 
This will continue until the capacitor has completely discharged, then the polarity of the capacitor will change as the inductor has created a reversed EMF, and then the entire cycle will repeat.
```desmos-graph
y=5\sin(4/(\pi) x)
```
## Charge
The charge of an L-C circuit is given by:
$$
\begin{aligned}
q(t)&= Q_0\cos(\omega t)\\
\hline\\
q&= \text{Charge}\\
Q_0&= \text{Initial Charge}\\
\omega&= \text{Frequency}\\
t&= \text{Time}
\end{aligned}
$$
## Current
This is the derivative of the charge, so this can be represented as:
$$
\begin{aligned}
i(t)&= -Q_0\omega\sin(\omega t)\\
\hline\\
q&= \text{Charge}\\
Q_0&= \text{Initial Charge}\\
\omega&= \text{Frequency}\\
t&= \text{Time}
\end{aligned}
$$
>[!Note]
>From this, we can see that the maximum [[Current]] is the maximum charge multiplied by the angular frequency
## Frequency
We can express the frequency of the oscillations with:
$$
\begin{aligned}
\omega&= \sqrt{\frac1{LC}}\\
\hline\\
\omega&= \text{Angular Frequency}\\
L&= \text{Inductance}\\
C&= \text{Capacitance}
\end{aligned}
$$
