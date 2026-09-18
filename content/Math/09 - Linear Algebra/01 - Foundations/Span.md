The **span** of a set $S$ is the **smallest [[Subspace]]** of a vector space $V$ that contains every vector in $S$.

We can think of the span as the set of **all possible [[Linear Combination|linear combinations]]** of the vectors in $S$.

For a set of vectors

$$
S=\{\vec u_1,\vec u_2,\ldots,\vec u_m\}\subseteq\mathbb R^n,
$$

the span is defined as

$$
\operatorname{span}(S)
=
\left\{
c_1\vec u_1+\cdots+c_m\vec u_m
\;\middle|\;
c_1,\ldots,c_m\in\mathbb R
\right\}.
$$

In other words, the span contains **every vector that can be created by taking a linear combination of the vectors in $S$**.

### Geometric Interpretation

The span describes the space that can be reached using the vectors in $S$.

For example:

* One non-zero vector can span a **line**.
* Two non-parallel vectors can span a **plane**.
* Three linearly independent vectors in $\mathbb R^3$ can span all of $\mathbb R^3$.

The vectors do **not** need to be orthogonal to span a space.

> [!Note]
> The span of any set of vectors in $\mathbb R^n$ is a [[Subspace]] of $\mathbb R^n$.
>
> The span can be written as
>
> $$
> \operatorname{span}(S)\subseteq\mathbb R^n.
> $$
>
> If the vectors in $S$ are [[Linear Independence|linearly independent]], then none of the vectors are redundant in describing the span.
