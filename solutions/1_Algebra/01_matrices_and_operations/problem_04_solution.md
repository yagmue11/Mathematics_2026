### Exercise 4. Matrix Multiplication and Noncommutativity

For

$$A= \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix},\qquad B= \begin{pmatrix} 2 & 0 \\ 3 & 1 \\ \end{pmatrix}$$

compute $AB$ and $BA$. Is $AB=BA$? Use this example to explain what noncommutativity of matrix multiplication means.

### Solution

**1. Computation of $AB$**

$$AB = \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 3 & 1 \\ \end{pmatrix}$$

Multiplying the rows of $A$ by the columns of $B$ yields:

$$AB = \begin{pmatrix} 8 & 2 \\ 3 & 1 \\ \end{pmatrix}$$

**2. Computation of $BA$**

$$BA = \begin{pmatrix} 2 & 0 \\ 3 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix}$$

Multiplying the rows of $B$ by the columns of $A$ yields:

$$BA = \begin{pmatrix} 2 & 4 \\ 3 & 7 \\ \end{pmatrix}$$

**3. Comparison and Explanation**

Comparing the resulting matrices, it is clear that:

$$AB \neq BA$$

This example demonstrates the noncommutativity of matrix multiplication. Unlike scalar multiplication where the order of operands does not matter (for example, $2 \cdot 3 = 3 \cdot 2$), changing the order of matrices in a product typically produces a completely different matrix. Therefore, the sequence of matrix factors must always be strictly preserved.