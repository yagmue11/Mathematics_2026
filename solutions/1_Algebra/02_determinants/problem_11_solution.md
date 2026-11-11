### Exercise 11. Shortening the Calculation with Row Operations

Compute

$$
\det \begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 4 \\
1 & 4 & 6
\end{pmatrix}
$$

by first performing row operations that create as many zeros as possible. State which operations do not change the determinant.

### Solution

**1. Apply row operations to create zeros**

To simplify the calculation, create zeros in the first column below the first entry.

- **Step 1:** Replace Row 2 with $R_2 - R_1$.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
1 & 4 & 6
\end{pmatrix}
$$

- **Step 2:** Replace Row 3 with $R_3 - R_1$.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix}
$$

**2. State which operations do not change the determinant**

The operation used in both steps is adding a scalar multiple of one row to another row. This specific row operation leaves the value of the determinant unchanged. Therefore, the determinant of the original matrix is equal to the determinant of the simplified matrix.

**3. Compute the determinant**

Using cofactor expansion along the first column of the simplified matrix:

$$
\det \begin{pmatrix}
1 & 2 & 3 \\
0 & 1 & 1 \\
0 & 2 & 3
\end{pmatrix} = 1 \cdot (1 \cdot 3 - 1 \cdot 2) - 0 + 0
$$

$$
\det A = 3 - 2 = 1
$$