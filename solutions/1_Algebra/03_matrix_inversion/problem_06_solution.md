### Exercise 6. Solving a System Using the Inverse

Solve

$$
A = \begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
,\qquad
b = \begin{pmatrix}
5 \\
7
\end{pmatrix}
$$

using $x=A^{-1}b$. Then substitute the resulting vector back into the equation and check the result.

### Solution

**1. Compute the inverse matrix $A^{-1}$**

The inverse of a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ is given by:

$$
A^{-1} = \frac{1}{\det A} \begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

First, compute the determinant of $A$:

$$
\det A = 2 \cdot 3 - 1 \cdot 1 = 6 - 1 = 5
$$

Applying the formula yields:

$$
A^{-1} = \frac{1}{5} \begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
$$

**2. Compute $x = A^{-1}b$**

$$
\begin{aligned}
x &= \frac{1}{5} \begin{pmatrix}
3 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
5 \\
7
\end{pmatrix} \\
&= \frac{1}{5} \begin{pmatrix}
3(5) + (-1)(7) \\
-1(5) + 2(7)
\end{pmatrix} \\
&= \frac{1}{5} \begin{pmatrix}
15 - 7 \\
-5 + 14
\end{pmatrix} \\
&= \begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix}
\end{aligned}
$$

**3. Verify by substitution**

Substitute the solution vector $x$ back into $Ax$:

$$
\begin{aligned}
Ax &= \begin{pmatrix}
2 & 1 \\
1 & 3
\end{pmatrix}
\begin{pmatrix}
\frac{8}{5} \\
\frac{9}{5}
\end{pmatrix} \\
&= \begin{pmatrix}
2\left(\frac{8}{5}\right) + 1\left(\frac{9}{5}\right) \\
1\left(\frac{8}{5}\right) + 3\left(\frac{9}{5}\right)
\end{pmatrix} \\
&= \begin{pmatrix}
\frac{16}{5} + \frac{9}{5} \\
\frac{8}{5} + \frac{27}{5}
\end{pmatrix} \\
&= \begin{pmatrix}
\frac{25}{5} \\
\frac{35}{5}
\end{pmatrix} \\
&= \begin{pmatrix}
5 \\
7
\end{pmatrix} = b
\end{aligned}
$$

Because $Ax = b$, the solution $x = \begin{pmatrix} \frac{8}{5} \\ \frac{9}{5} \end{pmatrix}$ is verified as correct.