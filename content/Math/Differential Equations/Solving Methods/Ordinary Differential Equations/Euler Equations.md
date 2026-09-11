These are a form of [[Second Order Differential Equation]] where there are variable coefficients, and these take the form:
$
$
\begin{aligned}
x^2y''+\alpha xy'+\beta y=\delta
\end{aligned}
$
$
We can solve this by guessing a solution. We guess with the form $y=x^r$. From here we can compute the first and second order derivatives, giving us:
$
$
\begin{aligned}
y& = x^2\\
y'&= rx^{r-1}\\
y''&= (r-1)rx^{r-2}
\end{aligned}
$
$
Subbing this back into the equation, we get:
$
$
\begin{aligned}
r^2+(\alpha-1)r+\beta=0
\end{aligned}
$
$
Which is also the [[Indicial Equation]].We can then solve this with the same form as a usual [[Second Order Differential Equation]]. Solving this for the two roots will give us an equation of the form:
$
$
\begin{aligned}
y(x)=\begin{cases}
Ax^{r_1}+Bx^{r_2}&\Delta >0\\
(A+B\ln x)x^r&\Delta =0\\
x^\lambda\Big(A\cos(\mu \ln x)+B\sin (\mu \ln x)\Big)&\Delta <0
\end{cases}
\end{aligned}
$
$
Where $\lambda=\frac{1-\alpha}2$ and $\mu=\frac{\sqrt{4\beta -(\alpha-1)^2}}2$.
>[!Note]
>If it is not a  [[Homogenous Equations]], then we can just solve for the [[Particular Solutions for Systems of Differential Equations]] the same way as usual. 

