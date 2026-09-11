This is any circuit that has a [[Resistor]] and a [[Capacitor]] in series
### Time Constant
This is how long it will take a [[Capacitor]] to reach $1-\frac1e$ of it's charge, or roughly $63.2\%$. The time constant is denoted by $\tau$. Thus, when $\tau$ is small, the charging takes less time and when $\tau$ is larger the charging will take more time. The time constant for an RC circuit is the product of the [[Resistance]] and the [[Capacitance]]:
>[!Note]
The definition of "charged" is after 5 time constants. 
$$
$$\begin{aligned}
\tau&= RC
\end{aligned}$$
$$
## Charging Capacitors
### Charge
When charging a [[Resistor]] when there is a battery and a [[Capacitor]] in series, as the battery charges the [[Capacitor]], then the increasing charge on the [[Capacitor]] will oppose the charge coming from the battery, therefore resisting the [[Voltage]]. This means that the longer it charges, the slower the flow rate is. Therefore, it is represented by the following equation:
$$
$$\begin{aligned}
q(t)&= \begin{cases}
C\mathcal{E}(1-e^{-\frac t\tau})\\
Q_0(1-e^{-\frac t\tau})
\end{cases}\\
\hline\\
q&= \text{Capacitor Charge}\\
\tau&= \text{Time Constant}\\
\mathcal{E}&= \text{Battery emf}\\
t&= \text{Time}\\
Q_0&= \text{Final Capacitor Charge}
\end{aligned}$$
$$
>[!Note]
>We can use $q(t)$ in the equation for the charge on a capacitor
### Instantaneous Current
The instantaneous [[Current]] flowing through the circuit is the time derivative of the equation above, or:
$$
$$\begin{aligned}
i(t)&= \begin{cases}
\frac{\mathcal{E}}{R}e^{-\frac t{\tau}}\\
I_0e^{-\frac t{\tau}}
\end{cases}\\
\hline\\
i&= \text{Current}\\
\tau&= \text{Time Constant}\\
\mathcal{E}&= \text{Battery emf}\\
t&= \text{Time}\\
Q_f&= \text{Final Capacitor Charge}
\end{aligned}$$
$$
## Discharging Capacitors
### Charge
Whenever a charged [[Capacitor]] is attached to a circuit and current is able to flow, we can express the [[Current]] at a given time with the following equation:
$$
$$\begin{aligned}
q&= Q_0e^{-\frac t{\tau}}\\
\hline\\
Q_0&= \text{Initial Capacitor Charge}\\
t&= \text{Time}\\
\tau&= \text{Time Constant}
\end{aligned}$$
$$
### Instantaneous Current
The following represents the [[Current]] at any time during the discharge of [[Capacitor]]:
$$
$$\begin{aligned}
i&= \begin{cases}
-\frac{Q_0}{\tau}e^{-\frac t{\tau}}\\
I_0e^{-\frac t{\tau}}
\end{cases}\\
\hline\\
Q_0&= \text{Initial Capacitor Charge}\\
I_0&= \text{Initial Current}\\
t&= \text{Time}\\
\tau&= \text{Time Constant}
\end{aligned}$$
$$
