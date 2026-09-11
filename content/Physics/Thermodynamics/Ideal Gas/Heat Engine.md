This is the concept of transforming [[Heat]] energy into useful mechanical energy. Anything that makes this transfer from [[Heat]] to mechanical is a heat engine.
>[!Note]
>No heat engine is ever 100% effective at converting from heat energy to mechanical energy, there is always a slight loss of energy to waste heat or friction. The amount of useful energy that comes out can be expressed as a percentage efficiency represented by the letter $e$:
>$$
$$
\begin{aligned}
\text{\% Efficiency}&= \frac{E_\text{out}}{E_\text{in}}\\
e&= \frac W{Q_H}
\end{aligned}
$$
$$

The matter that is inside of the heat engine is called the <u>working substance</u> of the engine. In fuel engines, this is the mixture of gasoline/diesel and air, in steam turbines it is water vapour. The working substance does the work by either releasing heat or by changing state. 
The simplest type of heat engine is one that undergoes a [[Volumetric Expansion]] process known as a cyclic process, where the [[Pressure Volume Processes]] undergoes a complete loop.
>[!Note]
>Because this is a cyclic process, the [[Internal Energy]] will not change over the whole loop, so we can rewrite the [[1st Law of Thermodynamics]] as:
>$$
$$
\begin{aligned}
Q&= W
\end{aligned}
$$
$$
## Temperature Reserves
While a heat engine works, there is useful [[Heat]] energy that comes from a heat reservoir, and waste heat that flows out into the cooler temperature reservoir. It is useful to think of these of not having any overall change in their own temperature, and rather just donates their heat to the engine (or accepts for the cold reservoir).
Because we can think of the cool reservoir as taking the energy away from the hot one, we can give it a negative sign and show it as the following:
$$
$$
\begin{aligned}
Q_\text{net}&= |Q_H|-|Q_C|
\end{aligned}
$$
$$
And because the work is equal to the net [[Heat]], we can express the work as:
$$
$$
\begin{aligned}
W&= Q_H|-|Q_C|
\end{aligned}
$$
$$
We can therefore also express efficiency as the following:
$$
$$
\begin{aligned}
e&= 1-\left|\frac{Q_C}{Q_H}\right|
\end{aligned}
$$
$$
## Otto Cycle
These is the [[Pressure Volume Processes]] that occur inside of combustion engines in cars. They are characterized by 4 [[Pressure Volume Processes]]:
1. [[Adiabatic]] Expansion
2. [[Isochoric]] Cooling
3. [[Adiabatic]] Compression
4. [[Isochoric]] Heating
### Efficiency
The efficiency of an otto cycle can be expressed by:
$$
$$
\begin{aligned}
e&= 1-\frac1{r^{\gamma-1}}\\
\hline\\
r&:\text{Compression Ratio}\\
\gamma&:\text{Radio of heat capacities}
\end{aligned}
$$
$$
With the usual values for compression ratio of gas ($r=8$) and the ratio of molar heat capacity ($\gamma=1.4$ for air), we get an efficiency of 56%. We can increase the efficiency by increasing the compression ratio or increasing the ratio of molar heat capacity. However, if the ratio of compression is raised too high, the gas will detonate and cause a knocking sound in the engine. 
>[!Note]
>Even though the theoretical value for efficiency is 56%, it is realistically lower due to friction, turbulence and other losses 
## Diesel Cycle
This is the same cycle as the Otto cycle, however instead of a isochoric heating as step 4, it has a [[Isobaric]] heating:
1. [[Adiabatic]] Expansion
2. [[Isochoric]] Cooling
3. [[Adiabatic]] Compression
4. [[Isobaric]] Heating
Diesel cycles also have no spark plugs, so there is no worry about false detonation, as detonation is what ignites the fuel. This causes the compression ratio to be much higher, around 15-20. This causes diesel engines to be more efficient than gasoline ones. This gives a diesel engine around 65% theoretical efficiency (lower in practice); however, diesel engines also require higher build quality and higher maintenance. 