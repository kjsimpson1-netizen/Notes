---
aliases:
---
These are also known as "op amps". These are [[Differential Amplifier|Differential Amplifiers]] where the gain, $A$, is extremely large (i.e. $A\to\infty$). These are important because we can make reliable circuits where the output is so large, even if there is uncertainty, it won't matter. The general equation for a voltage gain of a non inverting op amp is:
$$
\begin{aligned}
A_v=1+\frac{R_1}{R_2}
\end{aligned}
$$
## Negative Feedback
If there is a negative feedback loop in the circuit with the op-amp, then we can assume that the two input voltages ($V_p$ and $V_n$) are both equal, and that the two currents going in ($I_n$ and $I_p$) are both 0A. After this we then do a nodal analysis here.
## Buffer
This is another example of a negative feedback circuit, however with a direct loop from $V_\text{out}$ to $V_n$. This will cause the output of the op amp to always be equal to the voltage in. This converts a high output resistance into a low resistance source.
## Summing Amplifier
This is an [[Operational Amplifier|Amplifier]] that will sum together all of the input currents flowing