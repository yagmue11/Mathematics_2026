### Exercise 8. Two Systems with the Same Coefficient Matrix

Solve by elimination the two systems

$$
\begin{cases}
2x + y = 5, \\
x - y = 1,
\end{cases}
$$

$$
\begin{cases}
2x + y = 1, \\
x - y = 4.
\end{cases}
$$

Compare the successive elimination steps. Which part of the calculation is the same in both cases, and why?

### Solution

**1. Solve the first system**

Set up the augmented matrix for the first system:

$$
\begin{pmatrix}
2 & 1 & \mid & 5 \\
1 & -1 & \mid & 1
\end{pmatrix}
$$

Apply row operations to reach upper triangular form.

- **Step 1:** Swap Row 1 and Row 2 to place a $1$ in the pivot position.

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
2 & 1 & \mid & 5
\end{pmatrix}
$$

- **Step 2:** Replace Row 2 with $R_2 - 2R_1$.

$$
\begin{pmatrix}
1 & -1 & \mid & 1 \\
0 & 3 & \mid & 3
\end{pmatrix}
$$

Solve using back substitution:

$$
\begin{cases}
x - y = 1, \\
3y = 3.
\end{cases}
$$

From the second equation, $y = 1$. Substituting this into the first equation yields $x - 1 = 1$, so $x = 2$. The solution to the first system is the vector:

$$
\begin{pmatrix}
x \\
y
\end{pmatrix}
=
\begin{pmatrix}
2 \\
1
\end{pmatrix}
$$

**2. Solve the second system**

Set up the augmented matrix for the second system:

$$
\begin{pmatrix}
2 & 1 & \mid & 1 \\
1 & -1 & \mid & 4
\end{pmatrix}
$$

Apply the exact same sequence of row operations.

- **Step 1:** Swap Row 1 and Row 2.

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
2 & 1 & \mid & 1
\end{pmatrix}
$$

- **Step 2:** Replace Row 2 with $R_2 - 2R_1$.

$$
\begin{pmatrix}
1 & -1 & \mid & 4 \\
0 & 3 & \mid & -7
\end{pmatrix}
$$

Solve using back substitution:

$$
\begin{cases}
x - y = 4, \\
3y = -7.
\end{cases}
$$

From the second equation, $y = -\frac{7}{3}$. Substituting this into the first equation yields $x - \left(-\frac{7}{3}\right) = 4$, so $x + \frac{7}{3} = \frac{12}{3}$, meaning $x = \frac{5}{3}$. The solution to the second system is the vector:

$$
\begin{pmatrix}
x \\
y
\end{pmatrix}
=
\begin{pmatrix}
\frac{5}{3} \\
-\frac{7}{3}
\end{pmatrix}
$$

**3. Comparison and explanation**

The sequence of elementary row operations required to reduce the systems (swapping the rows, then subtracting twice the first row from the second) is identical in both cases.

This happens because the choice of row operations during Gaussian elimination is dictated entirely by the entries of the coefficient matrix. Because both systems share the exact same coefficient matrix, the structural steps required to reach upper triangular form are identical. The right-hand side vectors are merely carried along and passively transformed by these operations; they do not influence which operations are selected to eliminate the variables.