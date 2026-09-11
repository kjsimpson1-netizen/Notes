The [[Specific Heat]] of an ideal gas is determined by a closed system with a set volume (this is denoted by $C_V$). This is different than the way in which we measure the [[Specific Heat]] of solids and liquids, which is done at constant pressure (denoted by $C_P$. 
These are different due to the [[1st Law of Thermodynamics]]. Because if we keep the system at a constant volume, the work done by the system will be zero, whereas if we allow it to expand to keep the [[Pressure]] constant, the work will be positive, therefore changing the [[Internal Energy]] of the system as a whole. This means that the $C_V$ of a gas will be higher, do to the work that has to be done by the system. 
## Constant Volume
Considering the [[1st Law of Thermodynamics]], we can derive an equation for the change in temperature based off a change in energy for constant volume:
$
$
\begin{aligned}
dQ&= nC_V\;dT\\
\\
dU&= dQ-dW\\
dU&= dQ-0\\
\\
dU&= nC_V\;dT
\end{aligned}
$
$
## Constant Pressure
Because the [[Pressure]] must remain constant, the walls of the system must be allowed to expand to match to increasing [[Pressure]]. This means that gas does a nonzero amount of [[Work]] on the walls. We can represent the amount that the temperature changes based off an amount of energy put into the system for constant pressure systems based off of the following equation:
$
$
\begin{aligned}
dQ &= nC_P\;dT
\end{aligned}
$
$
The amount of work done by the gas is:
$
$
\begin{aligned}
dW&= p\;dV
\end{aligned}
$
$
We can substitute this into the [[Ideal Gas]] law, and because the pressure is constant, the temperature is based solely off of the change in volume:
$
$
\begin{aligned}
p\;dV&= nR\;dT
\end{aligned}
$
$
Putting both of these equations together into the [[1st Law of Thermodynamics]], we get the following equation:
$
$
\begin{aligned}
dU&= nC_P\;dT-nR\;dT
\end{aligned}
$
$
Because we declared the change in internal energy to be only directly proportional to the temperature and not based off of the pressure or the temperature, we can again use the same expression for $dU$ here:
$
$
\begin{aligned}
nC_V\;dT&= nC_P\;dT-nR\;dT
\end{aligned}
$
$
We can then factor out the $n\;dT$ out of each term to get the final expression for the relation between $C_V$ and $C_P$:
$
$
\begin{aligned}
C_P&= C_V+R
\end{aligned}
$
$
From this we can see that the pressure constant for specific heat is greater by approximately the gas constant (8.31). And it turns out that this is true for all gasses, not just ideal ones.
## Ratio of Heat Capacities
This is the ratio between the constant pressure and constant volume specific heats represented by the symbol $\gamma$. For monatomic gasses, $\gamma\approx1.67$, for diatomic $\gamma\approx1.40$ and for polyatomic $\gamma\approx 1.33$. This can be found by the fact that a monatomic gasses specific heat of constant volume can be represented by $\frac32R$. Plugging this into the equation above, we get the following:
$
$
\begin{aligned}
C_P&= C_V+R\\
&= \frac32R+R\\
&= \frac52R
\end{aligned}
$
$
Plugging this value into the equation for the ratio of heat capacities, we get the following:
$
$
\begin{aligned}
\gamma&= \frac{C_P}{C_V}\\
&= \frac{\frac52R}{\frac32R}\\
&= \frac53\\
&\approx 1.67
\end{aligned}
$
$
This is the same with diatomic gasses ($C_V=\frac73$)