### Exercise 2. Gaussian Elimination — One Solution

Solve using Gaussian elimination:

$$\begin{cases} x+y+z=6, \\ 2x-y+z=3, \\ x+2y-z=2. \end{cases}$$

After solving, substitute the result into all equations and check consistency.

### Solution

**1. Form the initial augmented matrix**

Extract the coefficients and constant terms into an augmented matrix:

$$\begin{pmatrix} 1 & 1 & 1 & \mid & 6 \\ 2 & -1 & 1 & \mid & 3 \\ 1 & 2 & -1 & \mid & 2 \\ \end{pmatrix}$$

**2. Apply row operations to reach upper triangular form**

* **Step 1:** Replace Row 2 with $R_2 - 2R_1$.

$$\begin{pmatrix} 1 & 1 & 1 & \mid & 6 \\ 0 & -3 & -1 & \mid & -9 \\ 1 & 2 & -1 & \mid & 2 \\ \end{pmatrix}$$

* **Step 2:** Replace Row 3 with $R_3 - R_1$.

$$\begin{pmatrix} 1 & 1 & 1 & \mid & 6 \\ 0 & -3 & -1 & \mid & -9 \\ 0 & 1 & -2 & \mid & -4 \\ \end{pmatrix}$$

* **Step 3:** Swap Row 2 and Row 3 to simplify calculations.

$$\begin{pmatrix} 1 & 1 & 1 & \mid & 6 \\ 0 & 1 & -2 & \mid & -4 \\ 0 & -3 & -1 & \mid & -9 \\ \end{pmatrix}$$

* **Step 4:** Replace Row 3 with $R_3 + 3R_2$.

$$\begin{pmatrix} 1 & 1 & 1 & \mid & 6 \\ 0 & 1 & -2 & \mid & -4 \\ 0 & 0 & -7 & \mid & -21 \\ \end{pmatrix}$$

**3. Solve using back substitution**

Write the corresponding upper triangular system:

$$\begin{cases} x + y + z = 6, \\ y - 2z = -4, \\ -7z = -21. \end{cases}$$

From the third equation, solve for $z$:

$$z = 3$$

Substitute $z = 3$ into the second equation to find $y$:

$$\begin{aligned} y - 2(3) &= -4 \\ y - 6 &= -4 \\ y &= 2 \end{aligned}$$

Substitute $y = 2$ and $z = 3$ into the first equation to find $x$:

$$\begin{aligned} x + 2 + 3 &= 6 \\ x + 5 &= 6 \\ x &= 1 \end{aligned}$$

The unique solution vector is:

$$\begin{pmatrix} x \\ y \\ z \\ \end{pmatrix} = \begin{pmatrix} 1 \\ 2 \\ 3 \\ \end{pmatrix}$$

**4. Check consistency by substitution**

Substitute $x=1$, $y=2$, and $z=3$ into the original equations to verify the result.

* **First equation:**

$$\begin{aligned} (1) + (2) + (3) &= 6 \\ 6 &= 6 \end{aligned}$$

* **Second equation:**

$$\begin{aligned} 2(1) - (2) + (3) &= 3 \\ 2 - 2 + 3 &= 3 \\ 3 &= 3 \end{aligned}$$

* **Third equation:**

$$\begin{aligned} (1) + 2(2) - (3) &= 2 \\ 1 + 4 - 3 &= 2 \\ 2 &= 2 \end{aligned}$$

Because substituting the values yields true statements for all three equations, the solution is verified as correct.