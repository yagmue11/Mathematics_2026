### Solution

**1. Computation of $A^T$ and $B^T$**

The transpose is found by swapping the rows and columns of each matrix:

$$A^T = \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \\ \end{pmatrix}$$

$$B^T = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \\ \end{pmatrix}$$

**2. Computation of $AB$ and $(AB)^T$**

First, compute the product $AB$:

$$AB = \begin{pmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix}$$

Multiplying the rows by the columns yields:

$$AB = \begin{pmatrix} 1(1) + 2(2) + 3(-1) & 1(0) + 2(1) + 3(3) \\ 4(1) + 5(2) + 6(-1) & 4(0) + 5(1) + 6(3) \\ \end{pmatrix}$$

$$AB = \begin{pmatrix} 2 & 11 \\ 8 & 23 \\ \end{pmatrix}$$

Taking the transpose of this result gives:

$$(AB)^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \\ \end{pmatrix}$$

**3. Computation of $B^T A^T$**

Now multiply the transposed matrices in reverse order:

$$B^T A^T = \begin{pmatrix} 1 & 2 & -1 \\ 0 & 1 & 3 \\ \end{pmatrix} \begin{pmatrix} 1 & 4 \\ 2 & 5 \\ 3 & 6 \\ \end{pmatrix}$$

Multiplying the rows by the columns yields:

$$B^T A^T = \begin{pmatrix} 1(1) + 2(2) - 1(3) & 1(4) + 2(5) - 1(6) \\ 0(1) + 1(2) + 3(3) & 0(4) + 1(5) + 3(6) \\ \end{pmatrix}$$

$$B^T A^T = \begin{pmatrix} 2 & 8 \\ 11 & 23 \\ \end{pmatrix}$$

**4. Verification**

Comparing the matrices from steps 2 and 3:

$$ (AB)^T = \begin{pmatrix} 2 & 8 \ 11 & 23 \ \end{pmatrix} = B^T A^T $$

This verifies that $(AB)^T = B^T A^T$ holds true for this example.