---
aliases:
  - Vector Fields
---
This is [[Vector]] valued function that will output a [[Vector]] at each point. For example:
$$
$$
\begin{aligned}
\vec v(x,y)
\end{aligned}
$$
$$
Will be a [[Vector]] function that takes $x$ and $y$ as arguments. 

---
A vector field on a plane is represented by:
$$
$$
\begin{aligned}
\vec F(x,y)&= P(x,y)\hat i+Q(x,y)\hat j
\end{aligned}
$$
$$
This can represent things such as velocity of wind on a map, strength of ocean currents, and other things that vary based off of location in 2 or 3 dimensional space. An example of this mathematically is the [[Gradient]].
>[!Definition]
>A [[Vector]] field $\vec F$ is called **conservative** if $\vec F=\nabla F$ for some $f(x,y)$ (called the potential function). This occurs if the [[Curl]] of the [[Vector Field]] is 0

However, we usually only draw the vector field restricted to a [[Surfaces|Surface]].
## Radial Vector Fields
These are vector fields which always point away from the origin, and their length is proportional to the distance from the origin. These take the form:
$$
$$
\begin{aligned}
\vec r(x,y)&= \langle x,y\rangle\\
|| \vec r||&= \sqrt{x^2+y^2+z^2}\\
\hat r=\frac{\vec r}{||r||}&= \left\langle\frac{x}{\sqrt{x^2+y^2+z^2}},\frac{y}{\sqrt{x^2+y^2+z^2}},\frac{z}{\sqrt{x^2+y^2+z^2}}\right\rangle
\end{aligned}
$$
$$
