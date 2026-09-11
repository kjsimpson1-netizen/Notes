## $e^x$
This is the only function that has a [[Derivative]] that is equal to the original function, or where the [[Slope]] at the evaluated point is equal to the function at that point. 
$$
$$
\begin{aligned}
\frac d{dx}e^x&= e^x
\end{aligned}
$$
$$
## $\ln x$
The [[Derivative]] of $\ln x$, or $\log_ex$, is equivalent to $\frac1x$
$$
$$
\begin{aligned}
\frac d{dx}\ln (\pm x)&= \frac1x
\end{aligned}
$$
$$
# Problematic Questions
## $\log_a x$
For these, you have to do a change of base to make it work 
$$
$$
\begin{aligned}
\log_ax&= \frac{\ln x}{\ln a}=\frac1{\ln a}\cdot\ln x\\\\
\frac d{dx}\log_ax&= \frac1{\ln a}\cdot\frac1x
\end{aligned}
$$
$$
## $y=a^x$
For these, you have to take the $\ln$ for both sides, then do [[Implicit Differentiation]]
$$
$$
\begin{aligned}
\ln y&= \ln a^x\\
\ln y&= x\cdot \ln a\\
\frac1y\cdot \frac{dy}{dx}&= \ln a\\
\frac{dy}{dx}&= \ln a\cdot y\\
\\
\frac{dy}{dx}&= a^x\cdot \ln a
\end{aligned}
$$
$$