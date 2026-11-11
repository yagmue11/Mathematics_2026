### Exercise 5. Row Operations

For

$$
A = \begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 0 \\
-1 & 4 & 2
\end{pmatrix}
$$

find $\det A$ by simplifying the matrix with row operations. At each step, indicate whether and how the determinant changes.

### Solution

**1. Apply row operations to reach upper triangular form**

- **Step 1:** Replace Row 2 with $R_2 - 2R_1$.
- **Effect on determinant:** Adding a scalar multiple of one row to another does not change the value of the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
-1 & 4 & 2
\end{pmatrix}
$$

- **Step 2:** Replace Row 3 with $R_3 + R_1$.
- **Effect on determinant:** Adding a scalar multiple of one row to another does not change the value of the determinant.

$$
\begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 6 & 5
\end{pmatrix}
$$

- **Step 3:** Replace Row 3 with $R_3 + 2R_2$.
- **Effect on determinant:** Adding a scalar multiple of one row to another does not change the value of the determinant.

$$
U = \begin{pmatrix}
1 & 2 & 3 \\
0 & -3 & -6 \\
0 & 0 & -7
\end{pmatrix}
$$

**2. Compute the determinant of the upper triangular matrix**

Since no operation altered the determinant value at any step, $\det A = \det U$.

The determinant of an upper triangular matrix is the product of its main diagonal entries:

$$
\det A = 1 \cdot (-3) \cdot (-7) = 21
$$