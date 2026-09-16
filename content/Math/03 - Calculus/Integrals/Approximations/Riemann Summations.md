Riemann summations are when the area under a function is estimated using rectangles of various sizes to estimate the area contained by the function (the [[Integral]]). The Riemann sums can be categorized by how many subintervals there are are a given [[Interval]], and which of the points of the rectangle is used as the height limit. 
The 4 approximation methods are:
1. RRAM (Right Rectangle Approximation Method)
2. LRAM (Left Rectangle Approximation Method)
3. MRAM (Middle Rectangle Approximation Method)
4. Trapezoid Approximation
>[!Note]
>The more rectangles that are added, the more accurate the approximation of the integral will be
## RRAM
RRAM (Right Rectangle Approximation Method) is when the height of the subdividing rectangle is set by where to right side of the rectangle (the right bound) is equal to the function. This is then multiplied by the [[Interval]] that the rectangle occurs on, and the amount of subdivisions dictates how wide the rectangle is for a specific sum. The area is the sum of all the rectangles, and the smaller the base of the rectangles, the more accurate the approximation. 
![[RRAM.png]]
We can also represent this using [[Summation Notation]], with the following format:
$$
\begin{aligned}
\int_a^bf(x)dx&\approx \left(\frac{b-a}{n}\right)\sum_{i=1}^nf\left(a+i\cdot\frac{b-a}n\right)\\
\hline\\
a&= \text{Lower Bound}\\
b&= \text{Upper Bound}\\
n&= \text{Steps}\\
f(x)&= \text{Function}
\end{aligned}
$$
## LRAM
LRAM (Left Rectangle Approximation Method) is when the height of the subdividing rectangle is set by where to left side of the rectangle (the left bound) is equal to the function. This is then multiplied by the [[Interval]] that the rectangle occurs on, and the amount of subdivisions dictates how wide the rectangle is for a specific sum. The area is the sum of all the rectangles, and the smaller the base of the rectangles, the more accurate the approximation. 
![[LRAM.png]]
We can also represent this using [[Summation Notation]], with the following format:
$$
\begin{aligned}
\int_a^bf(x)dx&\approx \left(\frac{b-a}{n}\right)\sum_{i=0}^{n-1}f\left(a+i\cdot\frac{b-a}n\right)\\
\hline\\
a&= \text{Lower Bound}\\
b&= \text{Upper Bound}\\
n&= \text{Steps}\\
f(x)&= \text{Function}
\end{aligned}
$$
This is the exact same as RRAM, however with the end points moved to the left. 
## MRAM
MRAM (Middle Rectangle Approximation Method) is when the height of the subdividing rectangle is set by where to centre side of the rectangle is equal to the function. This is then multiplied by the [[Interval]] that the rectangle occurs on, and the amount of subdivisions dictates how wide the rectangle is for a specific sum. The area is the sum of all the rectangles, and the smaller the base of the rectangles, the more accurate the approximation. 
![[MRAM.png]]
We can also represent this using [[Summation Notation]], with the following format:
$$
\begin{aligned}
\int_a^bf(x)dx&\approx \left(\frac{b-a}{n}\right)\sum_{i=1}^nf\left(a+\left(i-\frac12\right)\cdot\left(\frac{b-a}n\right)\right)\\
\hline\\
a&= \text{Lower Bound}\\
b&= \text{Upper Bound}\\
n&= \text{Steps}\\
f(x)&= \text{Function}
\end{aligned}
$$
## Limits of Riemann Summations
If we allow the number of sub rectangles tend to infinity, then the approximation will become more and more accurate.
$$
\begin{aligned}
\int_a^bf(x)dx&= \lim_{n\rightarrow\infty}\left(\frac{b-a}{n}\right)\sum\limits_{i=1}^nf\left(a+i\cdot\left(\frac{b-a}n\right)\right)\\
\hline\\
a&= \text{Lower Bound}\\
b&= \text{Upper Bound}\\
n&= \text{Steps}\\
f(x)&= \text{Function}
\end{aligned}
$$


