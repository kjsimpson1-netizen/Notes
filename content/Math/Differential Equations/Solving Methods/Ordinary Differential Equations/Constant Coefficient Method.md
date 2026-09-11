 For these problems, they will take the form of :
$$
$$
\begin{aligned}
y''+ay'+by&= C
\end{aligned}
$$
$$
Or the [[Homogeneity|Homogenous]] form:
$$
$$
\begin{aligned}
y''+ay'+by&= C
\end{aligned}
$$
$$
From here, we can take a guess that $y=e^{rx}$ and substitute this into the equation:
$$
$$
\begin{aligned}
r^2e^{rx}+are^{rx}+be^{rx}&= 0
\end{aligned}
$$
$$
From here, since all the coefficients are constants, we can then try [[Substitution]] with $y=e^{rx}$. We can then divide through by $e^{rx}$ to give us the *characteristic equation*:
$$
$$
\begin{aligned}
r^2+ar+b&= 0
\end{aligned}
$$
$$
>[!Note]
>$\Delta$ is the radicand of the [[Quadratic Equation]]
## $\Delta > 0$
So the solution will take the form:
$$
$$
\begin{aligned}
y=y_1+y_2= C_1e^{px}+C_2e^{qx}\qquad p,q\in\mathbb{R}
\end{aligned}
$$
$$
Where $p$ and $q$ are the roots of the [[Quadratic Equation]]:
## $\Delta = 0$
If there is a root with a multiplicity higher than 1, then we write the solution as:
$$
$$
\begin{aligned}
y(x)=(C_1+C_2x+C_3x^2...C_nx^{n-1})e^{px}
\end{aligned}
$$
$$
Where $p$ is the double root of the [[Quadratic Equation]]
## $\Delta < 0$
There are also cases where there are no real solutions to the characteristic equation, and in these cases we must use [[Complex Numbers]] to solve them. These types of answers can be expressed as:
$$
$$
\begin{aligned}
y=C_1e^{\alpha x}\cos(\beta x)+C_2e^{\alpha x}\sin(\beta x)
\end{aligned}
$$
$$
Where $\alpha$ and $\beta$ are the real number components in the [[Complex Numbers]]. 
## Combining Into a Single Form
We can change all these equations from the form of a $\sin$ and $\cos$ into a single $\cos$ by taking:
$$
$$
\begin{aligned}
C= \sqrt{C_1^2+C_2^2}&\qquad \gamma=\arctan\left(\frac {C_1}{C_2}\right)\\
\hline&\downarrow\\
x(t)&= C\cos(\beta t+\gamma)
\end{aligned}
$$
$$
However we can always just find that the constant $C$ will always be equal to the second coefficient of the characteristic equation.
>[!Warning]
>Be careful of the $\arctan$ function here, as it will always give an answer on the interval $[-\frac\pi2,\frac\pi2]$, and sometimes we want it to be on the other half of the unit circle

$$
$$
\begin{aligned}
\boxed{y(t) = e^{-t} \left( \cos(\sqrt{2} t) + \frac{1}{\sqrt{2}} \sin(\sqrt{2} t) \right)}
\end{aligned}
$$
$$
