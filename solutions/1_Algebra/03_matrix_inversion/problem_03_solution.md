### Exercise 3. When Does the Inverse Not Exist?

For

$$A= \begin{pmatrix} 2 & 4 \\ 1 & 2 \\ \end{pmatrix}$$

explain in two ways why $A^{-1}$ does not exist: using the determinant and using dependence between the rows.

### Solution

**1. Explanation using the determinant**

First, compute the determinant of $A$:

$$\det A = 2 \cdot 2 - 4 \cdot 1 = 0$$

A fundamental theorem of linear algebra states that a square matrix is invertible if and only if its determinant is non-zero. Because $\det A = 0$, the inverse matrix $A^{-1}$ does not exist.

**2. Explanation using dependence between the rows**

Let the rows of the matrix be denoted as $R_1$ and $R_2$:

$$\begin{aligned} R_1 &= (2, 4) \\ R_2 &= (1, 2) \end{aligned}$$

Comparing the two rows reveals that the first row is exactly twice the second row:

$$R_1 = 2R_2$$

Because one row is a scalar multiple of the other, the rows of the matrix are linearly dependent. A matrix is invertible if and only if its rows (and columns) are linearly independent. Due to this structural dependence, $A^{-1}$ does not exist.