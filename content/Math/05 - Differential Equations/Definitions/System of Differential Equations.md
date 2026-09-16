A first order system of [[Ordinary Differential Equations|ODE]]'s takes the form:
$$
\begin{aligned}
x'_1=f_1(t_1,x_0,...,x_n)\\
x'_2=f_1(t_1,x_0,...,x_n)\\
x'_n=f_1(t_1,x_0,...,x_n)
\end{aligned}
$$
Or in [[Vector]] form:
$$
\begin{aligned}
\vec x'&= \vec f(t_1,\vec x)(*)\\
\vec f&= \begin{pmatrix}
f_1\\
\vdots\\
f_n\\
\end{pmatrix}\qquad \vec x=\begin{pmatrix}
x_1\\ \vdots \\ x_n
\end{pmatrix}
\end{aligned}
$$
$\vec x$ is a continuous vector function that satisfies $*$
>[!Note]
>With higher [[Order]] [[Ordinary Differential Equations]], we can break this down into a lower degree function

We can also write this in [[matrix]] form:
$$
\begin{aligned}
\frac d{dx}\begin{pmatrix}
x_1\\x_2
\end{pmatrix}&= \begin{bmatrix}
1&2\\3&4
\end{bmatrix}\begin{pmatrix}
x_1\\ x_2
\end{pmatrix}+\begin{pmatrix}
1\\2
\end{pmatrix}=P(t)\vec x+\vec f(t)
\end{aligned}
$$
Where we set $\vec x(t)=(x_1(t),x_2(t))^T$.  We can then write the answer in the form:
$$
\begin{aligned}
\vec x(t)&= C_1\vec x_1(t)+C_2\vec x_2(t)+C_3\vec x_3(t)+...+C_n\vec x_n(t)
\end{aligned}
$$


