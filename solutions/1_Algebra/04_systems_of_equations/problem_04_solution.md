### Exercise 4. Infinitely Many Solutions

Solve

$$
\begin{cases}
x+y+z=2, \\
2x+2y+2z=4, \\
x-y+z=0.
\end{cases}
$$

Give the solution in parametric form, identify a free variable, and for one chosen parameter value check that the resulting point really satisfies the system.

### Solution

**1. Form the initial augmented matrix**

Extract the coefficients and constant terms into an augmented matrix:

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
2 & 2 & 2 & \mid & 4 \\
1 & -1 & 1 & \mid & 0
\end{pmatrix}
$$

**2. Apply row operations to reduce the system**

- **Step 1:** Replace Row 2 with $R_2 - 2R_1$.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
1 & -1 & 1 & \mid & 0
\end{pmatrix}
$$

- **Step 2:** Replace Row 3 with $R_3 - R_1$.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 0 & 0 & \mid & 0 \\
0 & -2 & 0 & \mid & -2
\end{pmatrix}
$$

- **Step 3:** Swap Row 2 and Row 3.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & -2 & 0 & \mid & -2 \\
0 & 0 & 0 & \mid & 0
\end{pmatrix}
$$

- **Step 4:** Multiply Row 2 by $-\frac{1}{2}$.

$$
\begin{pmatrix}
1 & 1 & 1 & \mid & 2 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0
\end{pmatrix}
$$

- **Step 5:** Replace Row 1 with $R_1 - R_2$.

$$
\begin{pmatrix}
1 & 0 & 1 & \mid & 1 \\
0 & 1 & 0 & \mid & 1 \\
0 & 0 & 0 & \mid & 0
\end{pmatrix}
$$

**3. Identify the free variable and write the parametric solution**

The pivot columns are columns 1 and 2 (corresponding to $x$ and $y$). Column 3 (corresponding to $z$) contains no pivot, so $z$ is the free variable.

Set $z = t$, where $t \in \mathbb{R}$. Expressing $x$ and $y$ in terms of the parameter $t$:

$$
\begin{cases}
x = 1 - t, \\
y = 1, \\
z = t.
\end{cases}
$$

In vector parametric form, the general solution is:

$$
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
1 \\
1 \\
0
\end{pmatrix}
+ t
\begin{pmatrix}
-1 \\
0 \\
1
\end{pmatrix},
\qquad t \in \mathbb{R}
$$

**4. Check for a chosen parameter value**

Choose the parameter value $t = 2$. This yields the specific point:

$$
\begin{pmatrix}
x \\
y \\
z
\end{pmatrix}
=
\begin{pmatrix}
1 - 2 \\
1 \\
2
\end{pmatrix}
=
\begin{pmatrix}
-1 \\
1 \\
2
\end{pmatrix}
$$

Substitute $x = -1$, $y = 1$, and $z = 2$ into all three original equations:

- **First equation:**

$$
\begin{aligned}
(-1) + (1) + (2) &= 2 \\
2 &= 2
\end{aligned}
$$

- **Second equation:**

$$
\begin{aligned}
2(-1) + 2(1) + 2(2) &= 4 \\
-2 + 2 + 4 &= 4 \\
4 &= 4
\end{aligned}
$$

- **Third equation:**

$$
\begin{aligned}
(-1) - (1) + (2) &= 0 \\
-2 + 2 &= 0 \\
0 &= 0
\end{aligned}
$$

All three equations are satisfied, verifying that the point belongs to the solution set.