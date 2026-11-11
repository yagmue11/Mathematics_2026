### Exercise 4. Matrix Multiplication and Noncommutativity

For

$$A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}, \qquad B = \begin{pmatrix} 2 & 0 \\ 3 & 1 \end{pmatrix}$$

compute $AB$ and $BA$. Is $AB = BA$? Use this example to explain what noncommutativity of matrix multiplication means.

### Solution

**1. Computation of $AB$**

$$AB = \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} \begin{pmatrix} 2 & 0 \\ 3 & 1 \end{pmatrix}$$

We compute each entry by taking the dot product of the rows of $A$ and the columns of $B$:

$$AB = \begin{pmatrix} (1)(2) + (2)(3) & (1)(0) + (2)(1) \\  (0)(2) + (1)(3) & (0)(0) + (1)(1) \end{pmatrix}$$

Simplifying each entry:

$$AB = \begin{pmatrix} 2 + 6 & 0 + 2 \\  0 + 3 & 0 + 1 \end{pmatrix} = \begin{pmatrix} 8 & 2 \\  3 & 1 \end{pmatrix}$$

---

**2. Computation of $BA$**

$$BA = \begin{pmatrix} 2 & 0 \\ 3 & 1 \end{pmatrix} \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix}$$

Similarly, we compute each entry by taking the dot product of the rows of $B$ and the columns of $A$:

$$BA = \begin{pmatrix} (2)(1) + (0)(0) & (2)(2) + (0)(1) \\  (3)(1) + (1)(0) & (3)(2) + (1)(1) \end{pmatrix}$$

Simplifying each entry:

$$BA = \begin{pmatrix} 2 + 0 & 4 + 0 \\  3 + 0 & 6 + 1 \end{pmatrix} = \begin{pmatrix} 2 & 4 \\  3 & 7 \end{pmatrix}$$

---

**3. Comparison and Explanation**

Comparing the resulting products:

$$AB = \begin{pmatrix} 8 & 2 \\ 3 & 1 \end{pmatrix} \quad \text{and} \quad BA = \begin{pmatrix} 2 & 4 \\ 3 & 7 \end{pmatrix}$$

Clearly, $AB \neq BA$.

This example demonstrates the **noncommutativity** of matrix multiplication. Unlike scalar multiplication—where the order of factors does not matter (for example, $2 \cdot 3 = 3 \cdot 2$)—matrix multiplication depends fundamentally on the order of the operands. Swapping the order of matrices in a product generally results in a completely different matrix, meaning the sequence of factors must always be strictly preserved.