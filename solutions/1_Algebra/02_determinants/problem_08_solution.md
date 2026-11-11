### Exercise 8. Determinant of a Product

Let $A,B$ be square matrices such that $\det A=3$ and $\det B=-5$. Compute $\det(AB)$, $\det(BA)$ and, if it exists, $\det(A^{-1}B)$. Explain why the first two results are equal even though usually $AB\neq BA$.

### Solution

**1. Compute $\det(AB)$ and $\det(BA)$**

The determinant is multiplicative, meaning the determinant of a matrix product is the product of their determinants.

$$
\det(AB) = \det A \cdot \det B = 3 \cdot (-5) = -15
$$

Similarly, for the reverse product:

$$
\det(BA) = \det B \cdot \det A = (-5) \cdot 3 = -15
$$

**2. Compute $\det(A^{-1}B)$**

Because $\det A = 3 \neq 0$, the matrix $A$ is invertible, meaning $A^{-1}$ exists. The determinant of an inverse matrix is the reciprocal of the original determinant.

$$
\begin{aligned}
\det(A^{-1}B) &= \det(A^{-1}) \cdot \det B \\
&= \frac{1}{\det A} \cdot \det B \\
&= \frac{1}{3} \cdot (-5) \\
&= -\frac{5}{3}
\end{aligned}
$$

**3. Explanation of equality**

While matrix multiplication itself is generally not commutative ($AB \neq BA$), the determinant function maps a square matrix to a single scalar number. Because the multiplication of real numbers is commutative, the order of the scalar factors does not matter:

$$
\det(AB) = \det A \cdot \det B = \det B \cdot \det A = \det(BA)
$$