This is a very useful tool for [[Math/09 - Linear Algebra/02 - Linear Systems/Linear System]]. It relies on the principle of being able to multiple an equation by a [[Scalar]] and have the product be a scaled version of the original, yet still be equal. The goal of Gaussian elimination is to get the vector into [[Row Echelon Form]] or [[Reduced Row Echelon Form]]. This can be done by either:

1. **Row Interchange**: Swap rows if needed to avoid zero pivots.
2. **Row Scaling**: Make the pivot element 1 (optional but simplifies calculations).
3. **Row Replacement**: Eliminate elements below the pivots.
4. **Forward Elimination**: Create zeros below each pivot in the [[Matrix]].
5. **Back Substitution**: Solve the system by substituting values starting from the bottom row.
---
>[!Note]
>If there are any rows with all zeroes, we place this row at the very bottom of the matrix. 
