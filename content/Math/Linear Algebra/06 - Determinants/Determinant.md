### Calculating Determinants Using Row Expansion

The **determinant** of a square [[Matrix]] can be calculated using **row expansion** (also called **cofactor expansion**). This method involves expanding along a row or column and recursively computing the determinants of smaller submatrices.
>[!Note]
>We can also use [[Determinant Operations]] before using the row operation to make the matrix simpler by creating more zeroes

---

#### Formula for Row Expansion
For an $n \times n$ [[Matrix]] $A$, the determinant can be computed by expanding along the $i$-th row:
$$
\det(A) = \sum_{j=1}^n (-1)^{i+j} a_{ij} \cdot \det(M_{ij}),
$$
where:
- $a_{ij}$ is the element in the $i$-th row and $j$-th column of $A$,
- $M_{ij}$ is the $(n-1) \times (n-1)$ submatrix obtained by deleting the $i$-th row and $j$-th column of $A$,
- $(-1)^{i+j}$ is the **cofactor sign**.

---

#### Steps for Row Expansion
1. **Choose a Row**: Select a row $i$ to expand along (typically the first row for simplicity).
2. **Compute Cofactors**: For each element $a_{ij}$ in the row, compute its cofactor:
   $$
   C_{ij} = (-1)^{i+j} \cdot \det(M_{ij}).
   $$
3. **Sum the Products**: Multiply each element $a_{ij}$ by its cofactor $C_{ij}$ and sum the results:
   $$
   \det(A) = \sum_{j=1}^n a_{ij} \cdot C_{ij}.
   $$
### Key Points:
- Row expansion works for matrices of any size but becomes computationally intensive for large matrices.
- The choice of row or column for expansion does not affect the result but can simplify calculations.
- If a row or column has many zeros, expanding along it can reduce the number of computations.