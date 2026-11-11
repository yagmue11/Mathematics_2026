### Exercise 5. A 3×3 Matrix

Use Gauss–Jordan elimination to find the inverse of

$$
A = \begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix}.
$$

Check the result by multiplication.

### Solution

**1. Form the initial augmented matrix**

Set up the augmented matrix $[A \mid I]$:

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
1 & 0 & 1 & \mid & 0 & 0 & 1
\end{pmatrix}
$$

**2. Apply row operations to reach $[I \mid A^{-1}]$**

- **Step 1:** Replace Row 3 with $R_3 - R_1$.

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & -1 & 1 & \mid & -1 & 0 & 1
\end{pmatrix}
$$

- **Step 2:** Replace Row 3 with $R_3 + R_2$.

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 2 & \mid & -1 & 1 & 1
\end{pmatrix}
$$

- **Step 3:** Multiply Row 3 by $\frac{1}{2}$.

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 1 & \mid & 0 & 1 & 0 \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

- **Step 4:** Replace Row 2 with $R_2 - R_3$.

$$
\begin{pmatrix}
1 & 1 & 0 & \mid & 1 & 0 & 0 \\
0 & 1 & 0 & \mid & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

- **Step 5:** Replace Row 1 with $R_1 - R_2$.

$$
\begin{pmatrix}
1 & 0 & 0 & \mid & \frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
0 & 1 & 0 & \mid & \frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
0 & 0 & 1 & \mid & -\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

**3. State the inverse matrix**

The matrix on the right side of the augmented system is $A^{-1}$:

$$
A^{-1} = \begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} & \frac{1}{2} \\
\frac{1}{2} & \frac{1}{2} & -\frac{1}{2} \\
-\frac{1}{2} & \frac{1}{2} & \frac{1}{2}
\end{pmatrix}
$$

This can also be written by factoring out the scalar:

$$
A^{-1} = \frac{1}{2} \begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix}
$$

**4. Check the result by multiplication**

Compute the product $AA^{-1}$ to verify it yields the identity matrix $I$.

$$
\begin{aligned}
AA^{-1} &= \begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1
\end{pmatrix} \cdot \frac{1}{2} \begin{pmatrix}
1 & -1 & 1 \\
1 & 1 & -1 \\
-1 & 1 & 1
\end{pmatrix} \\
&= \frac{1}{2} \begin{pmatrix}
1(1) + 1(1) + 0(-1) & 1(-1) + 1(1) + 0(1) & 1(1) + 1(-1) + 0(1) \\
0(1) + 1(1) + 1(-1) & 0(-1) + 1(1) + 1(1) & 0(1) + 1(-1) + 1(1) \\
1(1) + 0(1) + 1(-1) & 1(-1) + 0(1) + 1(1) & 1(1) + 0(-1) + 1(1)
\end{pmatrix} \\
&= \frac{1}{2} \begin{pmatrix}
2 & 0 & 0 \\
0 & 2 & 0 \\
0 & 0 & 2
\end{pmatrix} \\
&= \begin{pmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{pmatrix}
\end{aligned}
$$

Because $AA^{-1} = I$, the computed inverse is verified as correct.