### Exercise 11. Parameter and Invertibility

For

$$
A(t) = \begin{pmatrix}
1 & t \\
t & 1
\end{pmatrix}
$$

find all $t$ for which the matrix is invertible, and then give a formula for $A(t)^{-1}$. Explain what happens to this formula at the excluded values.

### Solution

**1. Find values of $t$ for which $A(t)$ is invertible**

A square matrix is invertible if and only if its determinant is non-zero.

First, compute the determinant of $A(t)$:

$$
\det A(t) = 1 \cdot 1 - t \cdot t = 1 - t^2
$$

Set the determinant to be non-zero:

$$
1 - t^2 \neq 0
$$

$$
t^2 \neq 1
$$

$$
t \neq \pm 1
$$

The matrix $A(t)$ is invertible for all real numbers $t$ except $t = 1$ and $t = -1$.

**2. Find the formula for $A(t)^{-1}$**

The inverse of a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ is given by:

$$
A^{-1} = \frac{1}{\det A} \begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

Substituting the entries of $A(t)$ and its determinant yields:

$$
A(t)^{-1} = \frac{1}{1 - t^2} \begin{pmatrix}
1 & -t \\
-t & 1
\end{pmatrix}
$$

or, carrying the scalar into the matrix:

$$
A(t)^{-1} = \begin{pmatrix}
\frac{1}{1-t^2} & -\frac{t}{1-t^2} \\
-\frac{t}{1-t^2} & \frac{1}{1-t^2}
\end{pmatrix}
$$

**3. Explain what happens at the excluded values**

At $t = 1$ and $t = -1$:

- **Algebraic effect:** The determinant becomes $1 - (\pm 1)^2 = 0$. The scalar factor $\frac{1}{1-t^2}$ requires division by zero and becomes undefined, causing the inverse formula to break down.
- **Structural effect:**
  - For $t = 1$, $A(1) = \begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix}$. The two rows are identical ($R_2 = R_1$).
  - For $t = -1$, $A(-1) = \begin{pmatrix} 1 & -1 \\ -1 & 1 \end{pmatrix}$. The second row is a scalar multiple of the first ($R_2 = -R_1$).

In both cases, the rows are linearly dependent, meaning the linear transformation maps the two-dimensional plane onto a one-dimensional line. Because this dimensional collapse destroys information, no inverse transformation can exist.