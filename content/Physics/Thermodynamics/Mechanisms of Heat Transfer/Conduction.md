This occurs when there are two objects directly in contact exchanging [[Heat]]. For example, when heating a metal rod the [[Heat]] travels through the metal via conduction. This is done by the atoms inside the materials transferring their energy to their neighbours. In conduction, the flow of [[Heat]] is always from hot to cold. 
$$\begin{align*}
H=\frac{dQ}{dt}=kA\frac{T_H-T_C}{L}
\end{align*}$$
Where:
$$\begin{align*}
H&= \text{Heat Current in Conduction}\\
dQ&= \text{Rate of heat flow}\\
k&=\text{Thermal Conductivity of material} 
\end{align*}$$
The term $\frac{T_H-T_C}{L}$ can be defined as the temperature gradient in unit length. 
Objects with high amounts of "dead" air (non-moving air) such as Styrofoam and fibreglass, which contain dead air, will have very small that the [[Thermal Resistance]] of them will be very low. 

There are also some materials that do not have a uniform heating pattern, and this can be fixed by introducing a new variable, $x$, along the length of the conductor. This can be represented by the equation:
$$\begin{align*}
H=\frac{dQ}{dt}=-kA\frac{dT}{dx}
\end{align*}$$
## Conductivity as a function of time
The rate of the flow of energy will decrease as time goes on, as the temperatures, which are the things that pushes the [[Heat]] through the system, will decrease in difference and therefore the fraction will decrease in magnitude, until the change is eventually 0, and the two objects are in [[Thermal Equilibrium]]. This only occurs if the two different temperatures are not defined as constant and are rather allowed to change. 
We can look at this as two temperatures, $T_1$ and $T_2$. The temperature of the two as a function of time, must be equal to the difference between the two temperatures as a function of time
$$\begin{align*}
T_{12}(t)&= T_1(t)-T_2(t)
\end{align*}$$
We cant then put this into the [[Conduction]] equation:
$$\begin{align*}
H&= kA\frac{T_1-T_2}L\\
&= kA\frac{T_{12}}L
\end{align*}$$
After a short time ($dt$), the energy that flows out of the block represented by $dQ_1$, which flows out of block 1.
$$\begin{align*}
H&= -\frac{dQ_1}{dt}\\
&= -\frac{mcdT_1}{dt}\\
\\
\frac{dT_1}{dt}&= -\frac{H}{mc}\\
&= -\frac{kA}{mcL}T_{12}
\end{align*}$$
Energy $dQ_2$ flows into block 2,  increasing it's temperature by $dT_2$:
$$\begin{align*}
H&= \frac{dQ_2}{dt}\\
&= \frac{mc\;dT_2}{dt}\\
\\
\rightarrow\frac{dT_2}{dt}&= \frac H{mc}
\end{align*}$$
We can then combine these two terms together:
$$\begin{align*}
\frac{dT_2}{dt}&= \frac{kA}{mcL}T_{12}
\end{align*}$$
The overall flow of [[Heat]] can be found by comparing the difference between these two rates of heat flow:
$$\begin{align*}
\frac{dT_{12}}{dt}&= \frac{dT_1}{dt}-\frac{dT_2}{dt}\\
&= -\frac{kA}{mcL}T_{12}-\frac{kA}{mcL}T_{12}\\
&= \left(-\frac{2kA}{mcL}\right)T_{12}
\end{align*}$$
We can then use calculus to get to the final step:
$$\begin{align*}
T_{12}(t)&= T_{12}(0)e^{-\frac{2kA}{mcL}t}
\end{align*}$$
![[Conduction.png]]
