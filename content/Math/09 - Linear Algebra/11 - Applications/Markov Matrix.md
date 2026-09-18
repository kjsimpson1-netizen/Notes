Considering a particle that jumps between 3 distinct states, we can use a [[Matrix Equation]] to describe this after $n\in \mathbb{R}$ jumps. 
This is denoted with $P_{ij}$, where $P$ is the probability that the particle jumps from state $j$ to state $i$. 
Since the probability must lie between 0% and 100%, each probability must lie between these values. Also, since there is a 100% chance that the particle will lie in one of the states:
$$
\begin{aligned}
P_{1j}+P_{2j}+P_{3j}&= 1
\end{aligned}
$$
Now, letting $x_i(n)$ be the probability of the particle being at state $i$ at time $n$, where $i\in\{1,2,3\}$ and $n\in\mathbb{I}$.

---
We can therefore say that the probability of finding the particle in state $i$ at $n+1$ is the sum of the probabilities of all the possible ways to get there, or:
$$
\begin{aligned}
x_i(n+1)&= P_{1i}x_{1}(n)+P_{2i}x_{2}(n)+P_{3i}x_{3}(n)
\end{aligned}
$$
We can then rewrite this as the following, known as a difference equation:
$$
\begin{aligned}
\vec x(n+1)=P\vec x(n)
\end{aligned}
$$
Therefore the function $x(n)$ only has a one step memory, as it only depends upon the time $n-1$, not $n-2$.

---
We can then express $P$ as:
$$
\begin{aligned}
P\equiv[P_{ij]}]=\begin{bmatrix}
P_{11}&P_{12}&P_{13}\\
P_{21}&P_{22}&P_{23}\\
P_{31}&P_{32}&P_{33}
\end{bmatrix}
\end{aligned}
$$
In which all of the columns of the [[Matrix]] must add up to one. Once we have this [[Matrix]], we can multiple it by the vector of the initial position, and then take whichever of the values we need for the particle of the current step:
$$
\begin{aligned}
\vec x(1)=P\vec x(0)=\begin{bmatrix}
P_{11}&P_{12}&P_{13}\\
P_{21}&P_{22}&P_{23}\\
P_{31}&P_{32}&P_{33}
\end{bmatrix}\begin{bmatrix}
0\\
1\\
0
\end{bmatrix}=
\begin{bmatrix}
P_{12}\\
P_{22}\\
P_{32}
\end{bmatrix}
\end{aligned}
$$
>[!Note]
>Initial position two was chosen here

We can then continue multiplying the by the current position probability for the necessary amount of times. 
## Equilibrium Value
The equilibrium value for a Markov matrix can be found using [[Eigenvalues]] and [[Eigenvalues|Eigenvectors]]. Every Markov matrix must have a [[Eigenvalues]] of 1, and the corresponding eigenvector will be the equilibrium matrix. We can also use the fact that the sum of the [[Eigenvalues]] is equal to the [[Trace]] to find the remaining [[Eigenvalues]]. 