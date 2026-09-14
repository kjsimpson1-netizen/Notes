A projection is a shadow of a [[Vector]] cast upon another vector, or the same as finding the magnitude of the vector that is going in the same direction as the original vector. The notation for this is "$\text{proj}_{\vec b}\vec a$", with the base "$\vec b$" being the vector that is being projected upon, and the "$\vec a$" is the vector being projected. 
![[Projections.png|697]]
$$\begin{align*}
\boxed{\text{Proj}_{\vec b}\vec a= (\vec a\cdot \vec b)\frac{\vec b}{||\vec b ||^2}}
\end{align*}$$
>[!Note]
>If $\vec b=\vec u$ is a unit vector (i.e. $||\vec u|| = 1$) then 
$$\begin{align*}
\boxed{\text{Proj}_{\vec b}\vec a= (\vec a\cdot \vec u)\vec u}
\end{align*}$$
## Projections onto planes
To do this, we take the perpendicular of the plane, $\vec n$ , and then project $\vec a$ onto it:
$$\begin{align*}
\text{Proj}_{\vec n}(\vec a)&= \vec a_\perp
\end{align*}$$
We can then use the difference between $\vec a$ and $\vec a_\perp$ to find the magnitude of $\vec a_\parallel$:
$$\begin{align*}
\boxed{\text{Proj}_S\vec a= \vec a-\text{Proj}_{\vec n}\vec a}
\end{align*}$$
