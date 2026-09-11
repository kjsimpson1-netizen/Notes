This is [[Simple Harmonic Motion]] where there is extra force that is acting against the restoring force. This is actually what happens to all objects that undergo [[Simple Harmonic Motion]], as no [[Periodic Motion]] can continue indefinitely as this would be perpetual motion.
## Damping due to Friction
We can represent the force due to friction with:
$$
$$\begin{aligned}
F_x&= -bv_x\\
\hline\\
F_x&= \text{Friction Force}\\
b&= \text{Damping Constant}\\
v_x&= \text{Velocity}
\end{aligned}$$
$$
Therefore, the net force on the system is:
$$
$$\begin{aligned}
F_\text{net}&= -kx-bv_x
\end{aligned}$$
$$
### Function of Time
We can also represent this as position as a function of time for the damped oscillator. This looks exactly like the equation for [[Simple Harmonic Motion]], however multiplied by a negative exponential to introduce the decay.
$$
$$\begin{aligned}
x(t)&= Ae^{-\frac b{2m}t}\cos(\omega't+\phi)\\
\hline\\
x&= \text{Position}\\
A&= \text{Initial Amplitude}\\
b&= \text{Damping Constant}\\
m&= \text{Mass}\\
\omega'&= \text{Angular Frequency}\\
\phi&= \text{Phase Angle}
\end{aligned}$$
$$
### Angular Frequency
We can represent the [[Angular Frequency]] of an damped oscillator with:
$$
$$\begin{aligned}
\omega'&= \sqrt{\frac km-\frac{b^2}{4m^2}}\\
\hline\\
\omega'&= \text{Anglar Frequency}\\
k&= \text{Force Constant}\\
m&= \text{Mass}\\
b&= \text{Damping Constant}
\end{aligned}$$
$$
>[!Note]
>The damped [[Angular Frequency]] is less than that of the undamped harmonic motion

## Types of Damping
Depending on the magnitude of the force, there are multiple different types of damping that can occur.
### Critical Damping
This is when the object is moved from [[Equilibrium Position]] and released, it returns directly to the resting position with no [[Periodic Motion Definitions]]. This occurs when one of the following is satisfied:
$$
$$\begin{aligned}
&\frac km-\frac{b^2}{4m^2}=0&&\text{or}&&b=2\sqrt{km}
\end{aligned}$$
$$
### Overdamping
This is also when there is no [[Oscillations]] and the object returns directly to the [[Equilibrium Position]], however this is slower than critical damping. This occurs when:
$$
$$\begin{aligned}
b>2\sqrt{km}
\end{aligned}$$
$$
The equation representing the motion of an overdamped oscillator is:
$$
$$\begin{aligned}
x(t)&= C_1e^{-a_1t}+C_2e^{-a_2t}
\end{aligned}$$
$$
In this equation, the constants $C_1$ and $C_2$ are determined by the initial conditions and $a_1$ and $a_2$ are constants determined by $m,k,$ and $b$.
### Under Damping
This is when the damping that occurs is less than the values to cause critical damping. Any object undergoing under damping will experience [[Simple Harmonic Motion]], however with decreasing [[Amplitude]].
## Energy
We can represent the change in energy of a damped oscillators with the following equation:
$$
$$\begin{aligned}
\frac{dE}{dt}&= -b{v_x}^2\\
\hline\\
\frac{dE}{dt}&= \text{Rate of change of Energy}\\
b&= \text{Damping Constant}\\
v_x&= \text{Velocity}
\end{aligned}$$ There is a negative sign, as the total energy of the system is decreasing as the amplitude of the oscillations decrease.
$$
