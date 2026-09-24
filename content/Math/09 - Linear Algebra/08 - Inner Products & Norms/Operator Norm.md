The operator norm is defined by:
$$\|A\| = \sup_{x\neq 0} \frac{\|Ax\|}{\|x\|}$$
This is an **induced norm** that measures the maximum stretch or amplification factor of a matrix/operator, rather than a direct element-wise analog of the vector [[Euclidean Norm]] (the direct analog is the [[Frobenius Norm]]).
Some key properties of the operator norm are:
1. $$\|A\| = \sup_{\|x\|=1} \|Ax\|$$
This measures the maximum distance $Ax$ can reach when $x$ lies on the unit sphere. It is **not** restricted to rotations; matrices can stretch, shear, or compress vectors.
2. If $A$ is an invertible square [[Matrix]], then:
$$\|A^{-1}\| = \frac{1}{\min_{\|x\|=1} \|Ax\|}$$

>[!NOTE]
>For standard $p$-norms ($\ell_1, \ell_2, \ell_\infty$), if $D$ is a [[Diagonal Matrix]], its operator norm is:
>$$\|D\| = \max_i |d_i|$$

### Requirements to be an Operator Norm
For a functional $\|A\|$ on linear operators $A: V \to W$ to be a valid operator norm, it must satisfy two sets of conditions:
1. **Vector Space Norm Axioms:**
   - **Definiteness:** $\|A\| \ge 0$, and $\|A\| = 0 \iff A = \mathbf{0}$
   - **Absolute Homogeneity:** $\|\alpha A\| = |\alpha| \cdot \|A\|$ for any scalar $\alpha$
   - **Triangle Inequality:** $\|A + B\| \le \|A\| + \|B\|$
2. **Operator & Submultiplicative Conditions:**
   - **Compatibility with Vector Norms:** $\|Ax\|_W \le \|A\| \cdot \|x\|_V$ for all $x \in V$
   - **Submultiplicativity:** For operators on the same space ($A, B: V \to V$), it must hold that:
     $$\|AB\| \le \|A\| \cdot \|B\|$$