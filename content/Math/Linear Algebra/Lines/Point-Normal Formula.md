This is similar to the [[Parametric Formula]], however using the normal direction as well. 
## 2 Dimensional
In the following, let $\vec p=(p_1,p_2)$ be the point and $\vec n=(n_1,n_2)$ be the normal direction.
$$\begin{align*}
\boxed{\vec n\cdot (\vec x-\vec p)= 0}
\end{align*}$$
This equation states that the difference between any two points is perpendicular to the [[Vector]] $\vec n$. This can also be rewritten as:
$$\begin{align*}
\boxed{\vec n\cdot \vec x=\vec n\cdot \vec p}
\end{align*}$$
## 3 Dimensional
This can also be used to express a line in 3 dimensions, however using the intersection line of two [[Planes]] in 3 dimensional space
>[!Warning]
>The [[Planes]] must not be parallel to each other

The equation for this is:
$$\begin{align*}
0&= \begin{cases}
\vec{n}_1\cdot(\vec x-\vec p)\\
\vec{n}_2\cdot(\vec x-\vec p)
\end{cases}\\
\hline\\
\vec{n}_1\cdot\vec x&= \vec n_1\cdot \vec p\\
\vec{n}_2\cdot\vec x&= \vec n_2\cdot \vec p
\end{align*}$$
You need to use both parameters because there are 3 degrees of freedom in 3D space. To reduce it to a line, you must constrain 2 of those 3 degrees of freedom. This is why two parameters are required to describe the line.
>[!Note]
>Since the line must be parallel to both [[Planes]], the [[Cross Product]] of the two normal directions of the planes will give the direction of the line

