### Exercise 15. Two Methods for Solving the Same System

For

$$A= \begin{pmatrix} 2 & 1 \\ 1 & 3 \\ \end{pmatrix},\qquad b= \begin{pmatrix} 7 \\ 8 \\ \end{pmatrix}$$

solve $Ax=b$ in two ways:

1. using $A^{-1}b$,
2. using Gaussian elimination.

Compare both solutions, the number of essential steps, and state which method was simpler in this example.

### Solution

**1. Method 1: Using $A^{-1}b$**

First, compute the determinant of $A$:

$$\det A = 2 \cdot 3 - 1 \cdot 1 = 5$$

Because the determinant is non-zero, the inverse exists. Apply the formula for the inverse of a $2 \times 2$ matrix:

$$A^{-1} = \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \\ \end{pmatrix}$$

Multiply $A^{-1}$ by the vector $b$:

$$\begin{aligned} x &= \frac{1}{5} \begin{pmatrix} 3 & -1 \\ -1 & 2 \\ \end{pmatrix} \begin{pmatrix} 7 \\ 8 \\ \end{pmatrix} \\ &= \frac{1}{5} \begin{pmatrix} 3(7) + (-1)(8) \\ -1(7) + 2(8) \\ \end{pmatrix} \\ &= \frac{1}{5} \begin{pmatrix} 21 - 8 \\ -7 + 16 \\ \end{pmatrix} \\ &= \frac{1}{5} \begin{pmatrix} 13 \\ 9 \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \\ \end{pmatrix} \end{aligned}$$

**2. Method 2: Gaussian elimination**

Set up the augmented matrix $[A \mid b]$:

$$\begin{pmatrix} 2 & 1 & \mid & 7 \\ 1 & 3 & \mid & 8 \\ \end{pmatrix}$$

Apply row operations to reach upper triangular form.

* **Step 1:** Swap Row 1 and Row 2.

$$\begin{pmatrix} 1 & 3 & \mid & 8 \\ 2 & 1 & \mid & 7 \\ \end{pmatrix}$$

* **Step 2:** Replace Row 2 with $R_2 - 2R_1$.

$$\begin{pmatrix} 1 & 3 & \mid & 8 \\ 0 & -5 & \mid & -9 \\ \end{pmatrix}$$

Solve the resulting upper triangular system using back substitution:

$$\begin{cases} x_1 + 3x_2 = 8, \\ -5x_2 = -9. \end{cases}$$

From the second equation:

$$x_2 = \frac{9}{5}$$

Substitute $x_2$ into the first equation:

$$\begin{aligned} x_1 + 3\left(\frac{9}{5}\right) &= 8 \\ x_1 + \frac{27}{5} &= \frac{40}{5} \\ x_1 &= \frac{40}{5} - \frac{27}{5} \\ x_1 &= \frac{13}{5} \end{aligned}$$

The solution vector is:

$$x= \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \\ \end{pmatrix}$$

**3. Comparison of both methods**

Both methods yield the exact same solution vector $x = \begin{pmatrix} \frac{13}{5} \\ \frac{9}{5} \end{pmatrix}$.

* The matrix inverse method required three essential steps: computing the determinant, constructing the inverse matrix, and performing the matrix-vector multiplication.
* Gaussian elimination also required three essential steps: setting up the augmented matrix, performing elimination via row operations, and evaluating the variables via back substitution.

For a specific numerical $2 \times 2$ system, the matrix inverse method is often conceptually simpler because the explicit formula for $A^{-1}$ allows for direct evaluation without tracking changing rows or solving algebraic equations backwards. However, Gaussian elimination avoids the intermediate construction of an inverse matrix altogether, making it much more computationally efficient and less error-prone for larger systems.