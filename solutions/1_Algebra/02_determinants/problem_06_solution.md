### Exercise 6. Parameter and Invertibility

For

$$A(t)= \begin{pmatrix} t & 1 \\ 2 & t \\ \end{pmatrix}$$

find all values of $t$ for which the matrix is not invertible. Explain how your answer is related to the determinant being zero.

### Solution

**1. Compute the determinant of $A(t)$**

$$\det A(t) = t \cdot t - 1 \cdot 2 = t^2 - 2$$

**2. Find values of $t$ for which the matrix is not invertible**

A square matrix is not invertible if and only if its determinant is equal to zero. Setting the determinant to zero and solving for $t$ yields:

$$t^2 - 2 = 0$$

$$t^2 = 2$$

$$t = \pm\sqrt{2}$$

The matrix $A(t)$ is not invertible for $t = \sqrt{2}$ and $t = -\sqrt{2}$.

**3. Explanation**

The inverse of a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ is given by the formula:

$$A^{-1} = \frac{1}{\det A} \begin{pmatrix} d & -b \\ -c & a \\ \end{pmatrix}$$

When $\det A(t) = 0$, the scalar multiplier $\frac{1}{\det A(t)}$ is undefined, meaning the inverse formula fails. Fundamentally, a determinant of zero indicates that the columns (or rows) of the matrix are linearly dependent. In this case, the matrix operation collapses the plane onto a line (or the origin), which is an irreversible transformation, meaning no inverse matrix can exist.