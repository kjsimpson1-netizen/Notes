We can solve a [[System of Differential Equations]] using the [[Matrix]]'s eigenvalues. We do this by first guessing a solution to the equation:
$$
\begin{aligned}
\vec x&= \vec ve^{\lambda t}\\
\frac d{dx}\vec x &=  \vec v\lambda e^{\lambda t}\\\\
\therefore \vec v\lambda \cancel{e^{\lambda t}}&= P\cdot\vec v\cancel{e^{\lambda t}}\\
\lambda\vec v&= P\vec v
\end{aligned}
$$
If we solve the equation above for the [[Eigenvalues]] using the [[Characteristic Equation]], we can find the answer to the equation. 

---
These are equations that relates at least one derivative of an unknown function $x(t)$ to other quantities that often include $x(t)$ itself. The order of these refer to the amount of derivatives that are present. 
>[!Note]
>For [[Linear Algebra]], we only like to have a single derivative, without higher degrees. This can be done by rewriting equations with higher degrees with only first order equations. 

## Second Degree
>[!Note]
We can also solve these using [[Matrix Exponentials]], as we can say that $\vec x'(t)=e^{At}\vec x_0$ where $A$ is the constant coefficient [[Matrix]]

We can rewrite a second degree ordinary differential equation as:
$$\begin{cases}
x_1'=a_{11}x_1(t)+a_{12}x_2(t)\\
x_2'=a_{21}x_1(t)+a_{22}x_2(t)
\end{cases}$$
We can make the following definitions:
$$
\begin{aligned}
\vec x(t)=
\begin{bmatrix}x_1(t)\\ x_2(t)\end{bmatrix}\qquad
\frac{d\vec x(t)}{dt}=\begin{bmatrix}
x_1'(t)\\x_2'(t)
\end{bmatrix}
\end{aligned}
$$
Therefore, we can rewrite the entire system as:
$$
\begin{aligned}
\begin{bmatrix}
x_1'(t)\\x_2'(t)
\end{bmatrix}=\begin{bmatrix}
a_{11}&a_{12}\\a_{21}&a_{22}
\end{bmatrix}\begin{bmatrix}
x_1(t)\\ x_2(t)
\end{bmatrix}
\end{aligned}
$$
Which is simplified to:
$$
\begin{aligned}
\frac{\vec x(t)}{dt}&= A\vec x(t),\qquad\text{A is a constant matrix}
\end{aligned}
$$
---
 
### Initial Conditions
For second order equations, we can state the following if it is a $2\times2$ matrix:
The solutions of the ordinary differential equation will be:
$$
\begin{aligned}
\vec x_1(t)= c_1e^{\lambda_1t}\vec v_1\qquad\vec x_2(t)= c_2e^{\lambda_2t}\vec v_2
\end{aligned}
$$
We can then just plug in the [[Eigenvalues]] and [[Eigenvalues|Eigenvectors]] for the equation. However, if we are given an initial value, then we can plug this in and either solve for it using a[[Math/09 - Linear Algebra/02 - Linear Systems/Linear System]]] or by using [[Inverse Matrices]]. We can then write this as:
$$
\begin{aligned}
\vec x&= \vec x_1+\vec x_2
\end{aligned}
$$

---
### Breaking up Complex Answers
We can break up the [[Complex Numbers|complex]] answers of the differential equation by adding and subtracting the [[Real Numbers|real]] and [[Imaginary Numbers|Imaginary]] parts of each of the differential equation answers. This is because if we add a complex number by it's complex conjugate, we get a real, and vice versa for subtraction. 
$$
\begin{aligned}
\vec x&= \vec x_1+\vec x_2=\text{Im}\{\vec v_1e^{\lambda_1t}\}+\text{Re}\{\vec v_1e^{\lambda_1t}\}
\end{aligned}
$$
We do this by taking $x_1$ and then factoring it into a form where we can rewrite it from [[Euler's Formula]] into the one including $\sin$ and $\cos$. 
$$
\begin{aligned}
\vec x_1&= c_1e^{\lambda_1t}\vec v_1\\
&= c_1e^{(a+bi)t}\vec v_1\\
&= c_1e^{at}e^{bti}\vec v_1\\
&= c_1e^{at}\left(\cos(bt)+\sin(bt)i\right)\vec v_1
\end{aligned}
$$
Multiplying this by the [[Eigenvalues|Eigenvectors]], we will get one column vector with reals and another with imaginaries . This can the be put into the form $a+bi$:
>[!Note]
>When we write the imaginary part of the differential equation, we can leave out the $i$, as the coefficient is a real number



