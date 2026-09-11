Any implicit equation has all the variables mixed together, while any explicit Equation has the 2 variables split up on both sides of the Equation. 
First, to solve these we can try and make into an explicit Equation by solving for y. But, if this isn't possible, we will need to use implicit differentiation. 

If it is not possible to make it into explicit differentiation, we can use the [[Chain Rule]] to evaluate with a variable that the derivative is not with respect to. 
>[!Note]
>We technically do implicit differentiation every time we take a derivative, with the left side of the equation being represented as follows:
>$$
\begin{aligned}
\frac d{dx}y&= 1\cdot \frac{dy}{dx}
\end{aligned}
$$
## Example

$$
\begin{aligned}
(x-2)^2+(y+3)^2&= 25
\end{aligned}
$$
This could be solved for $y$ and splitting it into two equations, however the implicit differentiation is more elegant
$$
\begin{aligned}
&& \frac d{dx}\Big[(x-2)^2+(y+3)^2\Big]&= \frac d{dx}\big[25\Big]&\textcolor{red}{\text{1. Taking the derivative of both sides}}&\\
&\implies&\frac d{dx}\Big[(x-2)^2\Big]+\frac d{dx}\Big[(y+3)^2\Big]&= 0\\
\\
\hline\\
&&\frac d{dx}\Big[(x-2)^2\Big]&= 2(x-2)&\textcolor{red}{\text{2. Derivatives of terms}}&\\
\\
&&\frac d{dx}\Big[(y+3)^2\Big]&= 2(y+3)\cdot\frac{dy}{dx}&\textcolor{red}{\text{2. Continued...}}\\
\\
\hline\\
&&&\therefore\\
&&2(x-2)+2(y+3)\cdot\frac{dy}{dx}&= 0&\textcolor{red}{\text{3. Substitution}}\\
&\implies&2x-4+(2y+6)\frac{dy}{dx}&= 0&\textcolor{red}{\text{4. Expansion of terms}}\\
&\implies&(2y+6)\frac{dy}{dx}&= -2x+4&\textcolor{red}{\text{5. Solving for }\frac{dy}{dx}}\\
&\implies&\frac{dy}{dx}&= -\frac{2x-4}{2y+6}&\textcolor{red}{\text{5. Continued...}}\\
&\implies&\frac{dy}{dx}&= -\frac{x-2}{y+3}&\textcolor{red}{\text{6. Simplification}}
\end{aligned}
$$
Because this [[Derivative]] has both of the variables in the solution, we must therefore evaluate at a point, rather than just an x value. We can see this is necessary because there are multiple different corresponding y values for a given x value. 
```desmos-graph
left = -4; right=9;
bottom = -10; top = 4;
---
(x-2)^2+(y+3)^2=25
```
## Evaluating Implicit Functions
For example, if we wanted to evaluate this at the point $(-2, 0)$, we would have to do it the following way:
$$
\begin{aligned}
&&\frac{dy}{dx}&= -\frac{x-2}{y+3}&\textcolor{red}{\text{1. Derivative}}\\
\\
\hline\\
&&\frac{dy}{dx}\Big|_{(-2,0)}&= -\frac{(-2)-2}{(0)+3}&\textcolor{red}{\text{2. Direct Subsitution}}\\
&\implies&&= \frac{4}{3}&\textcolor{red}{\text{3. Simplification}}
\end{aligned}
$$
