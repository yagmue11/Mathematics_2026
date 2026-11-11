### Exercise 10. Detecting Dependence

Without carrying out a full determinant calculation, explain why

$$
\det \begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 5
\end{pmatrix} = 0
$$

Identify a specific dependence between the rows and connect it with noninvertibility of the matrix.

### Solution

**1. Identify the dependence between the rows**

Let the rows of the matrix be denoted as $R_1$, $R_2$, and $R_3$. Comparing the first two rows yields:

$$
\begin{aligned}
R_1 &= (1, 2, 3) \\
R_2 &= (2, 4, 6)
\end{aligned}
$$

The second row is exactly twice the first row:

$$
R_2 = 2R_1
$$

**2. Explain why the determinant is zero**

Because one row is a scalar multiple of another, the rows of the matrix are linearly dependent. A fundamental property of the determinant function is that if the rows (or columns) of a square matrix are linearly dependent, its determinant is exactly zero.

Alternatively, this can be seen through row operations. Replacing the second row with $R_2 - 2R_1$ yields a matrix with an entire row of zeroes. The determinant of a matrix with a zero row is zero, and since this specific row operation does not change the determinant, the original determinant must also be zero.

**3. Connect dependence with non-invertibility**

A square matrix is invertible if and only if its determinant is non-zero. Because the linear dependence between the first and second rows forces the determinant to be zero, the matrix is not invertible.

In terms of linear transformations, the dependent rows indicate that the transformation maps the three-dimensional space onto a plane (a lower-dimensional space). This process loses information and cannot be reversed, which precisely means an inverse matrix cannot exist.