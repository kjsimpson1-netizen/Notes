When taking the conventional [[Inner Product]], we weight each of the entries with the same weight, usually $1$. However, if we care more about one section of the [[Inner Product]] being similar than others, we can add a **weight**. 
## Vectors
For vectors, this is the definition:
$$
\begin{aligned}
\braket{\vec v_1,\vec v_2}_W=\vec v_1^TW\vec v_2
\end{aligned}
$$
Where $W$ is a [[Diagonal Matrix]], with each entry representing how much we want to weigh each entry:
$$
\begin{aligned}
W = \begin{bmatrix} w_1 & 0 & 0 & \cdots & 0 \\ 0 & w_2 & 0 & \cdots & 0 \\ 0 & 0 & w_3 & \cdots & 0 \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & 0 & \cdots & w_n \end{bmatrix} = \text{diag}(w_1, w_2, w_3, \dots, w_n)
\end{aligned}
$$
## Function
For a function, this is given by a similar idea, however instead of multiplying by a [[Matrix]], we use another function, and this [[Inner Product]] will take the form:
$$
\begin{aligned}
\braket{f(x),g(x)}_W=\int_a^bw(x)f(x)g(x)dx
\end{aligned}
$$Where $w(x)$ is defined to be any function on the domain $x\in[a,b]$.