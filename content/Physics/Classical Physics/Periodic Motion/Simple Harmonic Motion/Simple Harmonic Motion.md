This is, as the name suggests, the simplest kind of periodic motion and the simplest [[Periodic Motion Definitions]]. This occurs when the force, $F_x$, is directly proportional to the displacement from the [[Equilibrium Position]] $x$. Any object that undergoes simple harmonic motion is a harmonic oscillator. This occurs with springs following [[Young's Modulus]]. This can be represented by the equation:
$$
\begin{aligned}
F_x&= -kx
\end{aligned}
$$
There is a negative here because the spring force is a restoring force, and it will return the object to the [[Equilibrium Position]]. 
For simple harmonic motion, we can show that the acceleration of the object is:
$$
\begin{aligned}
a_x&= \begin{cases}
-\frac kmx\\
-\omega^2x
\end{cases}\\
\hline\\
a&= \text{Acceleration}\\
k&= \text{Spring Constant}\\
m&= \text{Mass}\\
x&= \text{Position}\\
\omega&= \text{Angular Frequency}
\end{aligned}
$$
The negative sign here implies that the displacement from the [[Equilibrium Position]] and the acceleration of the object will always have opposite signs. 
>[!Note]
>Even though in many systems that undergo [[Simple Harmonic Motion]] the restoring force is not directly proportional to the displacement from the [[Equilibrium Position]], if the [[Amplitude]] is sufficiently small, it can be approximately proportional to the displacement and it can be used as an estimation

## Period and Frequency
For these objects, we can also represent the [[Angular Frequency]] with the following equation because it follows [[Simple Harmonic Motion]]:
$$
\begin{aligned}
\omega&= \sqrt\frac km\\
\hline\\
\omega&= \text{Angular Frequency}\\
k&= \text{Spring Constant}\\
m &=\text{Mass}
\end{aligned}
$$
We can also rewrite this in terms of [[Period]] and [[Frequency]]:
$$
\begin{aligned}
f&= \frac1{2\pi}\sqrt\frac km\\
T&= 2\pi\sqrt\frac km\\
\hline\\
\omega&= \text{Angular Frequency}\\
f&= \text{Frequency}\\
T&= \text{Period}\\
k&= \text{Spring Constant}\\
m &=\text{Mass}
\end{aligned}
$$
## Displacement
We can represent the position of the object undergoing [[Simple Harmonic Motion]] as a function of time with the following equation:
$$
\begin{aligned}
x(t)&= A\cos(\omega t+\phi)\\
\hline\\
x&= \text{Position}\\
A&= \text{Amplitude}\\
\omega&= \text{Angular Frequency}\\
\phi&= \text{Phase angle}
\end{aligned}
$$
The phase angle just tells us what the initial angle was at when $t=0$.
To find the velocity and the acceleration, we can take the derivative of the position function with respect to time:
$$
\begin{aligned}
&\text{Velocity}\\
v(t)&= -\omega A\sin(\omega t+\phi)\\
\\
&\text{Acceleration}\\
a(t)&= -\omega^2A\cos(\omega t+\phi)
\end{aligned}
$$
## Solving for phase angle and amplitude
By combining a few equations and solving for the variables above, we can express them with the following equations:
$$
\begin{aligned}
\phi&= \arctan\left(-\frac{v_{0x}}{\omega x_0}\right)\\
A&= \sqrt{{x_0}^2+\frac{{V_{0x}}^2}{\omega^2}}\\
\hline\\
\phi&= \text{Phase Shift}\\
v_{0_x}&= \text{Initial Velocity}\\
\omega&= \text{Angular Frequency}\\
x_0&= \text{Initial Position}\\
A&= \text{Amplitude}
\end{aligned}
$$
