### Exercise 2. Formula for a 2×2 Matrix

Find the inverse of

$$A= \begin{pmatrix} 3 & 2 \\ 5 & 4 \\ \end{pmatrix}$$

using the formula for a $2\times2$ matrix. At the end, check the result by computing one product with $A$.

> **Why this exercise:** teaches the simplest explicit formula for an inverse and requires verification using the definition.

### Solution

**1. Apply the formula for a $2 \times 2$ inverse**

The inverse of a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ is given by:

$$A^{-1} = \frac{1}{\det A} \begin{pmatrix} d & -b \\ -c & a \\ \end{pmatrix}$$

First, compute the determinant of $A$:

$$\det A = 3 \cdot 4 - 2 \cdot 5 = 12 - 10 = 2$$

Because $\det A \neq 0$, the inverse exists. Apply the formula by swapping the main diagonal entries, negating the off-diagonal entries, and multiplying by the scalar $\frac{1}{2}$:

$$\begin{aligned} A^{-1} &= \frac{1}{2} \begin{pmatrix} 4 & -2 \\ -5 & 3 \\ \end{pmatrix} \\ &= \begin{pmatrix} 2 & -1 \\ -\frac{5}{2} & \frac{3}{2} \\ \end{pmatrix} \end{aligned}$$

**2. Check the result by computing a product**

To verify, compute the product $AA^{-1}$ and check if it yields the identity matrix $I$.

$$\begin{aligned} A A^{-1} &= \begin{pmatrix} 3 & 2 \\ 5 & 4 \\ \end{pmatrix} \begin{pmatrix} 2 & -1 \\ -\frac{5}{2} & \frac{3}{2} \\ \end{pmatrix} \\ &= \begin{pmatrix} 3(2) + 2\left(-\frac{5}{2}\right) & 3(-1) + 2\left(\frac{3}{2}\right) \\ 5(2) + 4\left(-\frac{5}{2}\right) & 5(-1) + 4\left(\frac{3}{2}\right) \\ \end{pmatrix} \\ &= \begin{pmatrix} 6 - 5 & -3 + 3 \\ 10 - 10 & -5 + 6 \\ \end{pmatrix} \\ &= \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix} \end{aligned}$$

Because $AA^{-1} = I$, the computed inverse is correct.