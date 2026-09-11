---
aliases:
  - Amplifier
---
These are circuit components that can either step up or step down an incoming [[Voltage]] or [[Current]]. In general, these can only step up the input as high as the  source, and whenever it tries to go higher, it will clip out and no longer be able to amplify the value higher. We can represent this as a piecewise function:
$$
\begin{aligned}
V_\text{out}=\begin{cases}
V_{cc},\qquad&gV_{in}>V_{cc}\\
gV_{in}&gV_{in}\in[-V_{cc},V_{cc}]\\
-V_{cc},&gV_{in}<V_{cc}
\end{cases}
\end{aligned}
$$
## Operational Amplifier
These are also known as "op amps". These are differential amplifiers where the gain, $A$, is extremely large (i.e. $A\to\infty$). These are important because we can make reliable circuits where the output is so large, even if there is uncertainty, it won't matter. 