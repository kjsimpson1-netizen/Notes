This is when there is a mass on a spring and it oscillates following a [[Ordinary Differential Equations|ODE]] . The equation for this can be found from newtons first law. 
$$
$$
\begin{aligned}
m\ddot x+c\dot x+kx&= F_\text{net}\\
\hline\\
m&= \text{Mass}\\
x&= \text{Position}\\
k&= \text{Spring Constant}\\
c&= \text{Damping Constant}
\end{aligned}
$$
$$
This is a form of [[Ordinary Differential Equations]], and we can always just solve these equations via the [[Constant Coefficient Method]]
# Free Oscillations
## Damped Free Oscillations
In the equation above, if the $F_\text{net}$ is 0, this means that there is no force and the object is free to oscillate at the resonance frequency. This then takes the following form:
$$
$$
\begin{aligned}
mx''+cx'+kx&= 0\\
\implies x''+\frac cmx'+\frac kmx&= 0
\end{aligned}
$$
$$
And from physics, we have that $\frac km=\omega^2$, therefore we can write this as:
$$
$$
\begin{aligned}
\implies x''+\frac cmx'+\omega^2&= 0
\end{aligned}
$$
$$
The answer here depends on the sign of the determinant of the [[Quadratic Equation]].
### $\Delta > 0$, Overdamping
This occurs with a positive determinant. This equation can either decay to 0, or it can go through the equilibrium position exactly once, and this depends on the initial conditions:
$$
$$
\begin{aligned}
-\frac {C_1}{C_2}>0
\end{aligned}
$$
$$
If this is satisfied, then it will go through the equilibrium exactly once. 
### $\Delta =0$, Critical Damping
This occurs when there is a single root to the [[Quadratic Equation]], and this will approach 0 as $t\to\infty$ without crossing the x-axis. This is the fastest that the mass can approach the equilibrium position. 
### $\Delta<0$, Under Damped
This is when the determinant is negative and therefore this is a [[Complex Numbers]] root. This will still oscillate and approach the final value (think [[Sandwich Theorem]])
## Undamped Free Oscillations
This is when there is no force on the object, and there is no damping i.e. $c=0$. This gives us:
$$
$$
\begin{aligned}
mx''+kx&= 0\\
\implies x''+\frac kmx&= 0
\end{aligned}
$$
$$
And from physics, we have that $\frac km=\omega^2$, therefore we can write this as:
$$
$$
\begin{aligned}
x''+\omega ^2x&= 0
\end{aligned}
$$
$$
# Forced Oscillations
This is when the net force on the mass is not equal to 0, and therefore this will be a forced oscillation. This will take the form:
$$
$$
\begin{aligned}
mx''+kx=F_0\cos(\omega t)
\end{aligned}
$$
$$
### Driving Frequency is different
If the driving frequency is different than the resonance, we can write this as:
$$
$$
\begin{aligned}
x(t)&= C_1\cos(\omega_0t)+C_2\sin(\omega_0t)+\frac{F_0}{m(\omega_0^2-\omega^2)}\cos(\omega t)
\end{aligned}
$$
$$
>[!Note]
>This still applies providing that $\omega_0\neq\omega$, as otherwise there will be a division by 0 and the equation will blow up to infinity

```desmos-graph
\sin(x)*\sin(4x)
```

### Practical Resonance
This is when the oscillator can resonant with it's driving frequency, even with a damper. In order for this to exist, the following must be true:
$$
$$
\begin{aligned}
\omega^2_0-2p^2\ge0
\end{aligned}
$$
$$
This is because the frequency of the practical resonance is represented by:
$$
$$
\begin{aligned}
\omega_r=\sqrt{\omega_0^2-2p^2}
\end{aligned}
$$
$$
And the amplitude is:
$$
$$
\begin{aligned}
A(\omega)&= \frac{F_0}{m\sqrt{(\omega_n^2-\omega^2)^2+\left(\frac{c\omega}m\right)^2}}
\end{aligned}
$$
$$
