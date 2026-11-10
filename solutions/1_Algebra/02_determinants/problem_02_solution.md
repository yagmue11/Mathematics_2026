### Exercise 2. Determinant of a 3×3 Matrix

For

$$A= \begin{pmatrix} 1 & 2 & -1 \\ 0 & 3 & 4 \\ 2 & 1 & 5 \\ \end{pmatrix}$$

compute $\det A$ using Sarrus' rule. Then perform one simple check using a chosen property of the determinant.

### Solution

**1. Computation using Sarrus' rule**

By Sarrus' rule, the determinant is the sum of the products of the three main diagonals minus the sum of the products of the three anti-diagonals:

$$\begin{aligned} \det A &= (1)(3)(5) + (2)(4)(2) + (-1)(0)(1) - (-1)(3)(2) - (1)(4)(1) - (2)(0)(5) \\ &= 15 + 16 + 0 - (-6) - 4 - 0 \\ &= 31 - (-2) \\ &= 33 \end{aligned}$$

**2. Check using a property of the determinant**

A useful property of the determinant is that adding a scalar multiple of one row to another does not change its value. We can introduce a zero into the first column by subtracting $2$ times the first row from the third row ($R_3 \leftarrow R_3 - 2R_1$):

$$A' = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 3 & 4 \\ 0 & -3 & 7 \\ \end{pmatrix}$$

Because this row operation preserves the determinant, we can now compute the determinant of this new matrix by expanding along the first column:

$$\begin{aligned} \det A &= 1 \cdot \det \begin{pmatrix} 3 & 4 \\ -3 & 7 \\ \end{pmatrix} \\ &= 3(7) - 4(-3) \\ &= 21 - (-12) \\ &= 33 \end{aligned}$$

The results match, confirming the initial calculation.