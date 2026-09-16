To find the particular solution, one way is to use the undetermined coefficients method. This will take the general form:
$$
\begin{aligned}
A(x)y''+B(x)y'+C(x)y=f_0(x)+f_1(x)...
\end{aligned}
$$
From here, we choose a guess for the equation based off the of the $f(x)$ defined above, and we have to solve the particular solution for each of the forcing terms in isolation such as:
$$
\begin{aligned}
A(x)y''+B(x)y'+C(x)y&= f_0(x)\\
A(x)y''+B(x)y'+C(x)y&= f_1(x)\\
A(x)y''+B(x)y'+C(x)y&= ...
\end{aligned}
$$
We can then find the particular solutions following the guesses.

| $f(x)$                                                       | $y_p(x)$                                                                                                    |
| ------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| $P_n(x)=a_0+a_1x+a_2x^2+...+a_nx^n$                          | $x^s(A_0+A_1x+A_2x^2+...+A_nx^n)$                                                                           |
| $Q_n(x)=P_n(x)e^{\alpha x}$                                  | $x^s(A_0+A_1x+A_2x^2+...+A_nx^n)e^{\alpha x}$                                                               |
| $R_n(x)=P_n(x)e^{\alpha x}\ln(x)\cos(\beta x)$               | $x^s((A_0+A_1x+A_2x^2+...+A_nx^n)\cos(\beta x)+$<br>$(B_0+B_1x+B_2x^2+...+B_nx^n)\sin(\beta x)e^{\alpha x}$ |
| $S_n(x)=P_n(x)\cos(\omega x)\text{ or }P_n(x)\sin(\omega x)$ | $x^s(A\cos(\omega x)+B\sin(\omega x))$                                                                      |

>[!Note]
Where $s$ is the lowest possible integer such that the form of the guess does not contain any part of the two original branches of the [[Homogeneous Equations]].

From there we substitute it back into the original [[Non-Homogeneous Equations]] (taking derivatives where necessary) and solve for the coefficients $A$ and $B$. 
>[!Warning]
>We can only solve for the original constants of the [[Initial Conditions]] problem after we have added the particular and general solutions together following the steps for a [[Non-Homogeneous Equations]].

