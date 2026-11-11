### Exercise 12. A Parameter Revealed by a Row Operation

For

$$
A(t) = \begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & t \\
0 & 1 & 1
\end{pmatrix}
$$

find the values of $t$ for which the matrix is not invertible.

Before computing the determinant, perform the operation

$$
R_2 \leftarrow R_2 - 2R_1
$$

and use the resulting structure. At the end, explain what special thing happens to the rows for the value of the parameter you found.

### Solution

**1. Perform the specified row operation**

Replacing Row 2 with $R_2 - 2R_1$ yields a new matrix $B$:

$$
B = \begin{pmatrix}
1 & 2 & 3 \\
0 & 0 & t-6 \\
0 & 1 & 1
\end{pmatrix}
$$

Adding a scalar multiple of one row to another does not change the determinant, so $\det A(t) = \det B$.

**2. Compute the determinant**

Using cofactor expansion along the first column of the simplified matrix $B$:

$$
\begin{aligned}
\det B &= 1 \cdot \det \begin{pmatrix}
0 & t-6 \\
1 & 1
\end{pmatrix} \\
&= 1 \cdot (0 \cdot 1 - 1 \cdot (t-6)) \\
&= -(t-6) \\
&= 6 - t
\end{aligned}
$$

**3. Find values of $t$ for which the matrix is not invertible**

A square matrix is not invertible if and only if its determinant is equal to zero.

$$
6 - t = 0
$$

$$
t = 6
$$

The matrix $A(t)$ is not invertible when $t = 6$.

**4. Explanation of the row structure**

Substituting $t = 6$ into the original matrix yields:

$$
A(6) = \begin{pmatrix}
1 & 2 & 3 \\
2 & 4 & 6 \\
0 & 1 & 1
\end{pmatrix}
$$

For this specific parameter value, the second row is exactly twice the first row ($R_2 = 2R_1$). Because one row is a scalar multiple of another, the rows are linearly dependent. This structural dependence directly forces the determinant to be zero, rendering the matrix non-invertible.