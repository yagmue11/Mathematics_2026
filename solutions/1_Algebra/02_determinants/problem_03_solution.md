### Exercise 3. Swapping Two Rows

For

$$
A = \begin{pmatrix}
1 & 2 & 0 \\
0 & 3 & 1 \\
2 & 1 & 1
\end{pmatrix}
$$

compute $\det A$. Then form a matrix $B$ by swapping the first and second rows of $A$.

First predict $\det B$ using a determinant property, and then verify your prediction by calculation.

### Solution

**1. Compute the determinant of $A$**

Using cofactor expansion along the first row:

$$
\begin{aligned}
\det A &= 1 \cdot (3 \cdot 1 - 1 \cdot 1) - 2 \cdot (0 \cdot 1 - 1 \cdot 2) + 0 \\
&= 1 \cdot 2 - 2 \cdot (-2) \\
&= 2 + 4 \\
&= 6
\end{aligned}
$$

**2. Form matrix $B$ and predict its determinant**

Swapping the first and second rows of $A$ yields:

$$
B = \begin{pmatrix}
0 & 3 & 1 \\
1 & 2 & 0 \\
2 & 1 & 1
\end{pmatrix}
$$

A fundamental property of determinants states that swapping two rows of a square matrix multiplies its determinant by $-1$. Therefore, the prediction is:

$$
\det B = -\det A = -6
$$

**3. Verify the prediction by calculation**

Using cofactor expansion along the first row of $B$:

$$
\begin{aligned}
\det B &= 0 \cdot (2 \cdot 1 - 0 \cdot 1) - 3 \cdot (1 \cdot 1 - 0 \cdot 2) + 1 \cdot (1 \cdot 1 - 2 \cdot 2) \\
&= 0 - 3 \cdot 1 + 1 \cdot (1 - 4) \\
&= -3 + 1 \cdot (-3) \\
&= -6
\end{aligned}
$$

The direct calculation confirms the prediction.