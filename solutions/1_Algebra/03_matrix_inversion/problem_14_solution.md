### Exercise 14. A Matrix That Is Its Own Inverse

Assume that a square matrix $A$ satisfies

$$
A^2=I.
$$

Show that

$$
A^{-1}=A.
$$

Then give an example of a $2\times2$ matrix different from $I$ and $-I$ that satisfies this condition, and verify it by multiplication.

### Solution

**1. Show that $A^{-1}=A$**

The equation $A^2 = I$ can be written explicitly as a matrix product:

$$
AA = I
$$

By the definition of the inverse matrix, a square matrix $B$ is the inverse of $A$ if and only if $AB = BA = I$. Substituting $A$ for $B$ in this definition yields $AA = I$, which is exactly the given condition. Therefore, the matrix $A$ acts as its own inverse, meaning $A^{-1} = A$.

**2. Give a $2 \times 2$ matrix example**

A standard example of a matrix that is its own inverse is a reflection matrix. Consider the matrix representing a reflection across the line $y=x$:

$$
A = \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
$$

This matrix is explicitly different from both the identity matrix $I$ and its negation $-I$.

**3. Verify the example by multiplication**

Compute the product $A^2$ to verify that it yields the identity matrix $I$:

$$
\begin{aligned}
A^2 &= \begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix}
\begin{pmatrix}
0 & 1 \\
1 & 0
\end{pmatrix} \\
&= \begin{pmatrix}
0(0) + 1(1) & 0(1) + 1(0) \\
1(0) + 0(1) & 1(1) + 0(0)
\end{pmatrix} \\
&= \begin{pmatrix}
1 & 0 \\
0 & 1
\end{pmatrix}
\end{aligned}
$$

Because $A^2 = I$, the matrix satisfies the required condition.