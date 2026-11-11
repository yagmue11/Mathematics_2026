### Exercise 10. Inverse of a Diagonal Matrix

Given

$$
D = \begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
,\qquad
E = \begin{pmatrix}
2 & 0 & 0 \\
0 & 0 & 0 \\
0 & 0 & 5
\end{pmatrix}.
$$

Without using Gauss–Jordan elimination, decide which matrix is invertible. For the invertible matrix, give the inverse and check the result by multiplication.

### Solution

**1. Determine invertibility**

A diagonal matrix is invertible if and only if all of its main diagonal entries are non-zero.

For matrix $D$, the diagonal entries are $2$, $-3$, and $5$. Because none of these are zero, $D$ is invertible.

For matrix $E$, the second diagonal entry is $0$. Therefore, $E$ is not invertible.

**2. Find the inverse of $D$**

The inverse of an invertible diagonal matrix is obtained by replacing each main diagonal entry with its reciprocal:

$$
D^{-1} = \begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix}
$$

**3. Check the result by multiplication**

Compute the product $DD^{-1}$ to verify it yields the identity matrix $I$.

$$
\begin{aligned}
DD^{-1} &= \begin{pmatrix}
2 & 0 & 0 \\
0 & -3 & 0 \\
0 & 0 & 5
\end{pmatrix}
\begin{pmatrix}
\frac{1}{2} & 0 & 0 \\
0 & -\frac{1}{3} & 0 \\
0 & 0 & \frac{1}{5}
\end{pmatrix} \\
&= \begin{pmatrix}
2\left(\frac{1}{2}\right) & 0 & 0 \\
0 & -3\left(-\frac{1}{3}\right) & 0 \\
0 & 0 & 5\left(\frac{1}{5}\right)
\end{pmatrix} \\
&= \begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
\end{aligned}
$$

Because $DD^{-1} = I$, the computed inverse is verified as correct.