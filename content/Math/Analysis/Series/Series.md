This is an expression using [[Summation Notation]] and it is an expansion of [[Sequences]]. This is done by:
$$
$$
\begin{aligned}
\lim_{N\rightarrow\infty}S_N&= \lim_{n\rightarrow\infty}\sum_{n=0}^N a_n
\end{aligned}
$$
$$
If we have 2 series, each that have the limit of a real number, we are allowed to add, subtract and scalar multiply, however we cannot multiply series or divide them. 
## Indexing
We can also reindex a series by changing the term of the sequence that the series starts counting at, as well as changing the index. If we add one to the index, then we must subtract one from the sequence:
$$
$$
\begin{aligned}
\sum_{n=0}^\infty a_n=\sum_{n=1}^\infty a_{n-1}
\end{aligned}
$$
$$
Using this, we can use the series to back calculate the sequence using [[Partial Sum]], as:
$$
$$
\begin{aligned}
a_n=S_n-S_{n-1}
\end{aligned}
$$
$$
This is effectively taking the whole series, and subtracting every term from itself except the desired term. 