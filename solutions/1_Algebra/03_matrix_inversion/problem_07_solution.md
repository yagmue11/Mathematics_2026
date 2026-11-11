### Exercise 7. Inverse of a Product

For

$$
A = \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
,\qquad
B = \begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix}
$$

compute $(AB)^{-1}$ and $B^{-1}A^{-1}$. Check that the results are the same and explain the meaning of the reversed order.

### Solution

**1. Compute the product $AB$ and its inverse**

First, calculate the matrix product $AB$:

$$
\begin{aligned}
AB &= \begin{pmatrix}
1 & 1 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
2 & 0 \\
0 & 3
\end{pmatrix} \\
&= \begin{pmatrix}
1(2) + 1(0) & 1(0) + 1(3) \\
0(2) + 1(0) & 0(0) + 1(3)
\end{pmatrix} \\
&= \begin{pmatrix}
2 & 3 \\
0 & 3
\end{pmatrix}
\end{aligned}
$$

Next, find the inverse of $AB$. The determinant is $\det(AB) = 2 \cdot 3 - 3 \cdot 0 = 6$. Using the formula for the inverse of a $2 \times 2$ matrix yields:

$$
\begin{aligned}
(AB)^{-1} &= \frac{1}{6} \begin{pmatrix}
3 & -3 \\
0 & 2
\end{pmatrix} \\
&= \begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
\end{aligned}
$$

**2. Compute $B^{-1}A^{-1}$**

Find the individual inverses $A^{-1}$ and $B^{-1}$:

$$
A^{-1} = \begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix}
,\qquad
B^{-1} = \begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
$$

Multiply $B^{-1}$ and $A^{-1}$ in that specific order:

$$
\begin{aligned}
B^{-1}A^{-1} &= \begin{pmatrix}
\frac{1}{2} & 0 \\
0 & \frac{1}{3}
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
0 & 1
\end{pmatrix} \\
&= \begin{pmatrix}
\frac{1}{2}(1) + 0(0) & \frac{1}{2}(-1) + 0(1) \\
0(1) + \frac{1}{3}(0) & 0(-1) + \frac{1}{3}(1)
\end{pmatrix} \\
&= \begin{pmatrix}
\frac{1}{2} & -\frac{1}{2} \\
0 & \frac{1}{3}
\end{pmatrix}
\end{aligned}
$$

**3. Verify equality and explain the reversed order**

The computations confirm that $(AB)^{-1} = B^{-1}A^{-1}$.

The reversed order is required because matrix multiplication is not commutative. When applying the transformation $AB$ to a vector, the operation $B$ is applied first, followed by the operation $A$. To reverse this combined transformation, one must first undo the action of $A$ by applying $A^{-1}$, and then undo the action of $B$ by applying $B^{-1}$. Thus, the net inverse transformation is represented by the matrix product $B^{-1}A^{-1}$.