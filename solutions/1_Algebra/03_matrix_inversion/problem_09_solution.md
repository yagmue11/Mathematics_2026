### Exercise 9. Matrix Equation

Given

$$
A = \begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
,\qquad
B = \begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix}.
$$

Solve the equation $AX=B$ for $X$. Before calculating, decide on which side of the equation $A^{-1}$ must be used. Then check the result by computing $AX$.

### Solution

**1. Determine the algebraic step**

Because matrix multiplication is non-commutative, the position of the inverse matrix matters. To isolate $X$ in the equation $AX = B$, multiply both sides by $A^{-1}$ from the left:

$$
A^{-1}(AX) = A^{-1}B
$$

$$
(A^{-1}A)X = A^{-1}B
$$

$$
IX = A^{-1}B
$$

$$
X = A^{-1}B
$$

Multiplying from the right would yield $AXA^{-1} = BA^{-1}$, which does not isolate $X$.

**2. Compute $A^{-1}$**

For a $2 \times 2$ matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$, the inverse is given by:

$$
A^{-1} = \frac{1}{\det A} \begin{pmatrix}
d & -b \\
-c & a
\end{pmatrix}
$$

First, compute the determinant of $A$:

$$
\det A = 1 \cdot 1 - 2 \cdot 0 = 1
$$

Applying the formula yields:

$$
A^{-1} = \begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
$$

**3. Compute $X = A^{-1}B$**

$$
\begin{aligned}
X &= \begin{pmatrix}
1 & -2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix} \\
&= \begin{pmatrix}
1(3) + (-2)(2) & 1(1) + (-2)(4) \\
0(3) + 1(2) & 0(1) + 1(4)
\end{pmatrix} \\
&= \begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix}
\end{aligned}
$$

**4. Check the result by computing $AX$**

Substitute the matrix $X$ back into $AX$:

$$
\begin{aligned}
AX &= \begin{pmatrix}
1 & 2 \\
0 & 1
\end{pmatrix}
\begin{pmatrix}
-1 & -7 \\
2 & 4
\end{pmatrix} \\
&= \begin{pmatrix}
1(-1) + 2(2) & 1(-7) + 2(4) \\
0(-1) + 1(2) & 0(-7) + 1(4)
\end{pmatrix} \\
&= \begin{pmatrix}
3 & 1 \\
2 & 4
\end{pmatrix} = B
\end{aligned}
$$

Because $AX = B$, the computed matrix $X = \begin{pmatrix} -1 & -7 \\ 2 & 4 \end{pmatrix}$ is verified as correct.