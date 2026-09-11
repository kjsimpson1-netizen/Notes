 These are a method to find the [[Antiderivative]] of functions that can be broken down using the trigonometry functions. These identities are the ones that should be looked for while doing substitution:
$
$
\begin{aligned}
\sqrt{1-x^2}&&\sqrt{a^2+x^2}&&\sqrt{x^2-a^2}
\end{aligned}
$
$
We can use the following identities to find the antiderivative of the functions:
$
$
\begin{aligned}
1-\sin^2\theta&= \cos^2\theta&&1+\tan^2\theta= \sec^2
\end{aligned}
$
$
These can be rearranged into a form where they mimic the function under the root above. Each one has a corresponding substitution that must be made:
$
$
\begin{aligned}
\sqrt{a^2-x^2}&\implies \begin{cases}
x= a\sin\theta\\
dx= a\cos\theta d\theta
\end{cases}\\
\hline\\
\sqrt{a^2+x^2}&\implies \begin{cases}
x=a\tan\theta\\
dx=a\sec^2(\theta)d\theta
\end{cases}\\
\hline\\
\sqrt{x^2-a^2}&\implies \begin{cases}
x=a\sec\theta\\
dx= a\sec\theta\tan\theta d\theta
\end{cases}
\end{aligned}
$
$
---

## Examples
### Example 1
>[!Note] 
>Integration of $I = \int \sqrt{a^2 - x^2} \,dx$ assuming  $a \in \mathbb{R}^+$ .

$
$
\begin{aligned}
&\textbf{Step 1: Trigonometric Substitution} \\

&x = a\sin\theta, \quad dx = a\cos\theta \, d\theta \\

&a^2 - x^2 = a^2 - a^2\sin^2\theta = a^2\cos^2\theta \\
\hline\\
&\textbf{Step 2: Substituting into the Integral} \\

&I = \int \sqrt{a^2 - x^2} \, dx \\
&= \int \sqrt{a^2\cos^2\theta} \cdot a\cos\theta \, d\theta \\
&= a^2 \int \cos^2\theta \, d\theta \\
\hline\\
&\textbf{Step 3: Solve the Integral} \\

&= a^2 \int \frac{1 + \cos 2\theta}{2} \, d\theta \\
&= \frac{a^2}{2} \left( \theta + \frac{\sin 2\theta}{2} \right) + C \\
&= \frac{a^2}{2} \left( \theta + \sin\theta\cos\theta \right) + C \\
\hline\\
&\textbf{Step 4: Express in Terms of } x \\

&x = a\sin\theta \quad \Rightarrow \quad \sin\theta = \frac{x}{a} \\
&\theta = \arcsin\left(\frac{x}{a}\right) \\

&\cos^2\theta = 1 - \sin^2\theta = 1 - \left(\frac{x}{a}\right)^2 \\
&\cos\theta = \sqrt{1 - \left(\frac{x}{a}\right)^2} \\
\hline\\
&\textbf{Final Answer:} \\

&I = \frac{a^2}{2} \left( \arcsin\left(\frac{x}{a}\right) + \frac{x}{a} \sqrt{1 - \left(\frac{x}{a}\right)^2} \right) + C
\end{aligned}
$
$
### Example 2
$
$
\begin{aligned}
&\textbf{Step 1: Complete the Square} \\ 
&\text{The quadratic expression inside the square root is:} \quad 3 - 2x - x^2 \\ &\text{Rewriting in standard quadratic form:} \quad -(x^2 + 2x - 3) \\ &\text{Complete the square:} \\ &x^2 + 2x - 3 = (x+1)^2 - 4 \\ &\text{Thus, we rewrite the integral as:} \\ &I = \int \sqrt{-( (x+1)^2 - 4 )} \, dx \\ &I = \int \sqrt{4 - (x+1)^2} \, dx \\ 
\hline\\
&\textbf{Step 2: Trigonometric Substitution} \\ &\text{Let } x + 1 = 2\sin\theta \Rightarrow dx = 2\cos\theta \, d\theta \\ &\text{Then the expression under the square root simplifies:} \\ &4 - (x+1)^2 = 4 - 4\sin^2\theta = 4\cos^2\theta \\ &\text{Taking the square root:} \quad \sqrt{4\cos^2\theta} = 2\cos\theta \\ &\text{Now, substituting into the integral:} \\ &I = \int 2\cos\theta \cdot 2\cos\theta \, d\theta \\ &I = \int 4\cos^2\theta \, d\theta \\ 
\hline\\
&\textbf{Step 3: Solve the Integral} \\ &\text{Using the identity } \cos^2\theta = \frac{1 + \cos 2\theta}{2}, \text{ we rewrite:} \\ &I = \int 4 \cdot \frac{1 + \cos 2\theta}{2} \, d\theta \\ &I = \int (2 + 2\cos 2\theta) \, d\theta \\ &I = \int 2 \, d\theta + \int 2\cos 2\theta \, d\theta \\ &I = 2\theta + \sin 2\theta + C \\ 
\hline\\
&\textbf{Step 4: Substitute Back in Terms of } x \\ &\text{From our substitution } x + 1 = 2\sin\theta, \text{ so } \sin\theta = \frac{x+1}{2} \\ &\text{Using } \sin 2\theta = 2\sin\theta\cos\theta, \text{ and } \cos\theta = \sqrt{1 - \sin^2\theta}, \text{ we get:} \\ &\cos\theta = \sqrt{1 - \left(\frac{x+1}{2}\right)^2} = \frac{\sqrt{3 - 2x - x^2}}{2} \\ &\sin 2\theta = 2 \sin\theta \cos\theta = 2 \times \frac{x+1}{2} \times \frac{\sqrt{3 - 2x - x^2}}{2} \\ &= \frac{(x+1) \sqrt{3 - 2x - x^2}}{2} \\ 
\hline\\
&\textbf{Final Answer:} \\ &I = 2\sin^{-1} \left( \frac{x+1}{2} \right) + \frac{(x+1) \sqrt{3 - 2x - x^2}}{2} + C
\end{aligned}
$
$
### Example 3
>[!Note] 
>Using trigonometric substitution to evaluate $I = \int \frac{1}{\sqrt{x^2 - 4^2}} \,dx$.

$
$
\begin{aligned}
&\textbf{Step 1: Given Integral} \\
I &= \int \frac{1}{\sqrt{x^2 - 4^2}} \,dx \\
\hline\\

&\textbf{Step 2: Use Identity} \\
\sec^2\theta - 1 &= \tan^2\theta \\
\hline\\

&\textbf{Step 3: Trigonometric Substitution} \\
x &= 4\sec\theta \\
dx &= 4\sec\theta\tan\theta \, d\theta \\
\hline\\

&\textbf{Step 4: Substitute into the Integral} \\
I &= \int \frac{1}{\sqrt{4^2\sec^2\theta - 4^2}} \cdot 4\sec\theta\tan\theta \, d\theta \\
&= \int \frac{1}{4\sqrt{\sec^2\theta - 1}} \cdot 4\sec\theta\tan\theta \, d\theta \\
&= \int \frac{1}{4\tan\theta} \cdot 4\sec\theta\tan\theta \, d\theta \\
&= \int \sec\theta \, d\theta \\
&= \log|\sec\theta + \tan\theta| + C \\
\hline\\

&\textbf{Step 5: Back-Substituting} \\
\frac{x}{4} &= \sec\theta \\
\tan\theta &= \sqrt{\sec^2\theta - 1} \\
&= \sqrt{\left(\frac{x}{4}\right)^2 - 1} \\
\hline\\

&\textbf{Step 6: Final Answer} \\
I &= \log\left|\frac{x}{4} + \sqrt{\left(\frac{x}{4}\right)^2 - 1}\right| + C
\end{aligned}
$
$
