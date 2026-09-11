This is a method to break down [[Rational Functions]] into more simple forms that is useful to make taking the [[Antiderivative]] more easy. These can be found systematically in a few different ways, depending upon the degree of the polynomial
## Proper Fractions
This is when the numerator is less than the denominator, whether it be the magnitude or the degree
$$
\begin{aligned}
\frac{p(x)}{l_1(x)l_2(x)\dots l_n(x)}&= \frac A{l_1(x)}+\frac B{l_2(x)}+...
\end{aligned}
$$
In this form, we want to solve for the constant $A,B,\dots$ 
### Example
$$
\begin{aligned}
\frac6{w(w-w)(w-2)}&= \frac Aw+\frac B{w-1}+\frac C{w-2}\\
6&= {A(w-1)(w-2)}+B(w)(w-2)+C(w)(w-1)
\end{aligned}
$$
We then set the variable $w$ equal to the numbers which will make each of the fractions equal to 0.
$$
\begin{aligned}
&w=0&6=2A\\
&w=1&6=-B\\
&w=2&6=6C
\end{aligned}
$$
Therefore $A=3,B=-6,C=1$.
## Improper Fractions
This is when the numerator is larger degree than the denominator, and in this case we must do long division to make it into a proper fraction. This can be done by taking the quotient of the leading terms, then multiple this by the denominator and subtracting this from the numerator:
### Example
$$
\begin{aligned}
\frac{2x^2}{x^2+2}
\end{aligned}
$$
1. Step one: Taking the quotient
$$
\begin{aligned}
\frac{2x^2}{x^2}&= 2
\end{aligned}
$$
2. Multiply this by the denominator and subtract:
   $$
\begin{aligned}
2x^2-2(x^2+2)&= 2x^2-2x^2-4\\
&= -4
\end{aligned}
$$
3. Rewrite:   
$$
\begin{aligned}
-\frac4{x^2+x}+2
\end{aligned}
$$
This can now be done the same as a proper fraction. 