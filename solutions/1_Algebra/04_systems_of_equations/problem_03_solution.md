### Exercise 3. Inconsistent System

Solve or show that the system is inconsistent:

$$
\begin{cases}
x + 2y = 3, \\
2x + 4y = 7.
\end{cases}
$$

Show how the contradiction appears in the matrix after elimination and interpret it in terms of equations.

### Solution

**1. Form the initial augmented matrix**

Extract the coefficients and constant terms into an augmented matrix:

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
2 & 4 & \mid & 7
\end{pmatrix}
$$

**2. Apply row operations**

- **Step 1:** Replace Row 2 with $R_2 - 2R_1$.

$$
\begin{pmatrix}
1 & 2 & \mid & 3 \\
0 & 0 & \mid & 1
\end{pmatrix}
$$

**3. Interpret the contradiction**

Translate the resulting augmented matrix back into a system of linear equations:

$$
\begin{cases}
x + 2y = 3, \\
0x + 0y = 1.
\end{cases}
$$

The second equation simplifies to:

$$
0 = 1
$$

This equation is a logical contradiction, meaning there are no values of $x$ and $y$ that can satisfy it. Because the second equation cannot be satisfied, the entire system has no solution, proving that the system is inconsistent. In terms of the original equations, the two lines are parallel and never intersect.