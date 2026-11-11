### Exercise 1. Definition of the Inverse

For

$$
A = \begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
,\qquad
B = \begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
$$

check, without using a formula, whether $B=A^{-1}$. Compute $AB$ and $BA$ and relate the result to the definition of the inverse.

### Solution

**1. Compute the product $AB$**

$$
\begin{aligned}
AB &= \begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix}
\begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix} \\
&= \begin{pmatrix}
2(1) + 1(-1) & 2(-1) + 1(2) \\
1(1) + 1(-1) & 1(-1) + 1(2)
\end{pmatrix} \\
&= \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\end{aligned}
$$

**2. Compute the product $BA$**

$$
\begin{aligned}
BA &= \begin{pmatrix}
1 & -1 \\
-1 & 2
\end{pmatrix}
\begin{pmatrix}
2 & 1 \\
1 & 1
\end{pmatrix} \\
&= \begin{pmatrix}
1(2) + (-1)(1) & 1(1) + (-1)(1) \\
-1(2) + 2(1) & -1(1) + 2(1)
\end{pmatrix} \\
&= \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\end{aligned}
$$

**3. Relate to the definition of the inverse**

By definition, a matrix $B$ is the inverse of a square matrix $A$ if and only if their product in either order yields the identity matrix $I$.

Because the computations show that:

$$
AB = BA = \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix} = I
$$

it is confirmed that $B = A^{-1}$.