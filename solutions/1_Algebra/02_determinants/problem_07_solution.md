### Exercise 7. Using Properties Instead of Recomputing

Suppose that for a $3\times3$ matrix, $\det A=-4$. Compute

$$
\det(2A),\qquad \det(A^T),\qquad \det(A^2),\qquad \det(-A)
$$

Justify each answer using the appropriate property.

### Solution

**1. Compute $\det(2A)$**

When an $n \times n$ matrix is multiplied by a scalar $c$, the determinant is multiplied by $c^n$. This is because the scalar is factored out from each of the $n$ rows. For a $3 \times 3$ matrix, $n=3$ and the scalar is $c=2$.

$$
\begin{aligned}
\det(2A) &= 2^3 \det A \\
&= 8 \cdot (-4) \\
&= -32
\end{aligned}
$$

**2. Compute $\det(A^T)$**

The determinant of a matrix is equal to the determinant of its transpose.

$$
\det(A^T) = \det A = -4
$$

**3. Compute $\det(A^2)$**

The determinant is multiplicative, meaning $\det(AB) = \det A \cdot \det B$. Applying this to $A^2$ yields $\det(A^2) = (\det A)^2$.

$$
\begin{aligned}
\det(A^2) &= (\det A)^2 \\
&= (-4)^2 \\
&= 16
\end{aligned}
$$

**4. Compute $\det(-A)$**

Using the same scalar multiplication property from the first part, $-A$ is equivalent to scaling $A$ by $-1$. For a $3 \times 3$ matrix, this factors out as $(-1)^3$.

$$
\begin{aligned}
\det(-A) &= (-1)^3 \det A \\
&= -1 \cdot (-4) \\
&= 4
\end{aligned}
$$