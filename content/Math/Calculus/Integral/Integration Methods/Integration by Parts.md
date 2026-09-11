This is the integration equivalent of the [[Product Rule]], and must be done to take the [[Antiderivative]] of any [[Product Rule]]. The formal notation of this using [[Leibniz Notation]] is:
$$
$$\begin{aligned}
\int udv&= uv-\int vdu
\end{aligned}$$
$$
Where we can decide what our expressions for $u$ and $v$ will be. The expression for $u$ should be easily differentiable, and the expression for $v$ should have a simple [[Antiderivative]]. However, we also want to simplify the integral as much as possible and should take the most complicated part of the function to be differentiated.

---
## Examples
### Example 1
$$
$$\begin{aligned}
&\textbf{Integration by Parts:} \quad \int x \cos(x) \, dx \\
\hline\\
&\text{Using the formula:} \quad \int u \, dv = uv - \int v \, du \\ 
&\textbf{Step 1: Choose } u \text{ and } dv \\ 
&u = x \quad \Rightarrow \quad du = dx \\ 
&dv = \cos(x) \, dx \quad \Rightarrow \quad v = \int \cos(x) dx = \sin(x) \\
\hline\\
&\textbf{Step 2: Apply the formula} \\ &I = \int x \cos(x) \, dx \\ 
&I = u v - \int v \, du \\ 
&I = x \sin(x) - \int \sin(x) dx \\ 
&\text{Since } \int \sin(x) dx = -\cos(x), \text{ we get:} \\ 
&I = x \sin(x) + \cos(x) + C \\ 
\hline\\
&\textbf{Final Answer:} \quad \int x \cos(x) \, dx = x \sin(x) + \cos(x) + C
\end{aligned}$$
$$
### Example 2
#### Integration of $e^{\sqrt{x}}$

We will integrate $e^{\sqrt{x}}$ using first a $u$-substitution and then integration by parts (IBP).

##### Step 1: Use $u$-substitution
Let $u = \sqrt{x}$, so that $u^2 = x$ and $2u \, du = dx$ or $dx = 2u \, du$.

Now, substitute into the integral:

$$
\int e^{\sqrt{x}} \, dx = \int e^u \cdot 2u \, du
$$

##### Step 2: Integration by parts (IBP)
Recall the formula for integration by parts:

$$
\int v \, dw = vw - \int w \, dv
$$

In our case, we choose:
- $v = u$, so that $dv = du$.
- $dw = e^u \cdot 2 \, du$, so that $w = 2e^u$.

Now apply the IBP formula:

$$
\int e^u \cdot 2u \, du = 2u \cdot e^u - \int 2e^u \, du
$$

##### Step 3: Simplify the remaining integral
The integral of $2e^u$ is straightforward:

$$
\int 2e^u \, du = 2e^u
$$

So, the expression becomes:

$$
2u \cdot e^u - 2e^u = 2e^u (u - 1)
$$

##### Step 4: Substitute back $u = \sqrt{x}$
Finally, substitute $u = \sqrt{x}$ back into the expression:
$$
2e^{\sqrt{x}} (\sqrt{x} - 1) + C
$$
Thus, the final result is:

$$
\int e^{\sqrt{x}} \, dx = 2e^{\sqrt{x}} (\sqrt{x} - 1) + C
$$
$$
\begin{aligned}
&\textcolor{blue}{\textbf{Step 1: Choose } u \text{ and } dv} \\
&\quad \text{Let } u = x, \quad dv = \cos(x) \, dx. \\
&\textcolor{blue}{\textbf{Step 2: Compute } du \text{ and } v} \\
&\quad \text{Then } du = dx, \quad v = \sin(x). \\
&\textcolor{blue}{\textbf{Step 3: Apply integration by parts}} \\
&\quad \int u \, dv = uv - \int v \, du \quad \text{(Integration by parts formula)} \\
&\quad \implies \int x \cos(x) \, dx = x \sin(x) - \int \sin(x) \, dx. \\
&\textcolor{blue}{\textbf{Step 4: Simplify the integral}} \\
&\quad \int \sin(x) \, dx = -\cos(x) + C. \\
&\textcolor{blue}{\textbf{Step 5: Substitute back}} \\
&\quad \implies \int x \cos(x) \, dx = x \sin(x) - (-\cos(x)) + C. \\
&\textcolor{blue}{\textbf{Step 6: Finalize the result}} \\
&\quad \therefore \int x \cos(x) \, dx = x \sin(x) + \cos(x) + C.
\end{aligned}
$$
$$
