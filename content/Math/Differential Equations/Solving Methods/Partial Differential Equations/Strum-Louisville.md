This is the most general form of the solution for [[Partial Differential Equations]]. These will take the form:
$$
\begin{aligned}
\mathcal{L}\phi&= \lambda w(x)\phi
\end{aligned}
$$
This is valid on the domain from $x\in(0,l)$. It has the boundary conditions (also known as <u> seperated boundary conditions</u>):
$$
\begin{aligned}
\begin{cases}
\phi'(0)-h_1\phi(0)=0\\
\phi'(l)-h_1\phi(l)=0
\end{cases}
\end{aligned}
$$
Where $L\phi\equiv-[p(x)\phi']'+q(x)$
Assume for regular [[Strum-Louisville]] that:
$$
\begin{aligned}
\begin{cases}
p(x)>0&&x\in[0,l]\\
w(x)>0&&x\in[0,l]\\
p,q,w,h,h_1\in\mathbb{R}
\end{cases}
\end{aligned}
$$
>[!Note]
>$w(x)$ is called the "weight function"

[[Separation of Variables]] is a special case of [[Strum-Louisville]]