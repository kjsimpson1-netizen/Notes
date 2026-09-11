This is a variation of the [[Power Series Solutions]] to [[Partial Differential Equations]], however when there are [[Regular Singular Points]]. In order to solve these, after that we have confirmed that the [[Singular Point]] is regular, we can take the values of the two limits of the [[Regular Singular Points]] as $x\to x_0$, and then plug these two values of $\alpha$ and $\beta$ into the [[Indicial Equation]] and from there we can solve for the value of $r$. We can then plug it into the form:
$$
$$\begin{aligned}
y(x)=\sum_{n=0}^\infty a_nx^{n+r}
\end{aligned}$$
$$
Which is essentially a regular power series solution, however incorporating the [[Euler Equations]] 
>[!Note]
>The initial term of $a$ (i.e. $a_0$) will always be non zero
## Solving
Since we solve the [[Indicial Equation]] for the value of $r$, there will be two values for $r$, then we take $|r_1-r_2|$, This will give us a few different cases of how to solve:
***
#### $|r_1-r_2|\in\mathbb{Q^+}\land\notin\mathbb{Z}$ 
For this case, we will have that the two solutions will take the form of:
$$
$$\begin{aligned}
y(x)=\sum_{n=0}^\infty a_nx^{n+r_1}+\sum_{n=0}^\infty b_nx^{n+r_2}
\end{aligned}$$
$$
***
#### $|r_1-r_2|=0$
For this case, we will have the solution be of the form:
$$
$$\begin{aligned}
y(x)=(\ln(x)+1)\sum_{n=0}^\infty a_nx^{n+r_1}+\sum_{n=0}^\infty b_nx^{n+r_2}
\end{aligned}$$
$$
Once we get the general solution for $y_1(x,\lambda)$, then to find the second solution we will have to do the following:
$$
$$\begin{aligned}
y_2(x)&= \frac{\partial}{\partial \lambda }(y_1(x,\lambda))\Big|_{\lambda=0}
\end{aligned}$$
$$
***
#### $|r_1-r_2|\in\mathbb{N}$
For this case, the solution will take the form:
$$
$$\begin{aligned}
y(x)=(a\ln(x)+1)\sum_{n=0}^\infty a_nx^{n+r_1}+\sum_{n=0}^\infty b_nx^{n+r_2}
\end{aligned}$$
$$
In order to find the solution for this case, we will first try the [[Frobenius Method]] with $r_2$. From this point, there are 2 subcases:
##### $a_n\in\mathbb{R}:n\in\mathbb{N^+}$
In this case, we can just plug in the values of $a_n$ and everything works out nicely
##### $a_n\notin\mathbb{R}\forall n\in\mathbb{N^+}$
In this case, we have a blowup in one of the coefficients of $a_n$ (usually $a_0$ or $a_1$). In this case, we will have to use the root of the [[Indicial Equation]] that is well defined to then extrapolate the other solution. To find this solution, we will have that:
$$
$$\begin{aligned}
y_2=\frac{\partial }{\partial \lambda}(\lambda -\lambda _2)y(x,\lambda)\Big|_{\lambda=\lambda_2}
\end{aligned}$$
$$
Using the general case that is solved for leaving $\lambda$ as a general variable. After substituting in, we will see that the [[Regular Singular Points]] are removed. 
