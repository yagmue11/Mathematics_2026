### Exercise 2. Addition and Scalar Multiplication

For

$$A= \begin{pmatrix} 1 & 2 \\ -1 & 3 \\ \end{pmatrix},\qquad B= \begin{pmatrix} 4 & -2 \\ 0 & 5 \\ \end{pmatrix}$$

compute

$$A+B,\qquad A-B,\qquad 3A-2B.$$

Explain why matrix addition is possible only for matrices of the same size.

> **Why this exercise:** reinforces entry-by-entry operations and the importance of compatible dimensions.

### Exercise 2. Solution

**1. Computation of $A+B$**

$$A+B = \begin{pmatrix} 5 & 0 \\ -1 & 8 \\ \end{pmatrix}$$

**2. Computation of $A-B$**

$$A-B = \begin{pmatrix} -3 & 4 \\ -1 & -2 \\ \end{pmatrix}$$

**3. Computation of $3A-2B$**

First, compute the scalar multiplications:

$$3A = \begin{pmatrix} 3 & 6 \\ -3 & 9 \\ \end{pmatrix}$$

$$2B = \begin{pmatrix} 8 & -4 \\ 0 & 10 \\ \end{pmatrix}$$

Subtracting the two matrices yields:

$$3A-2B = \begin{pmatrix} -5 & 10 \\ -3 & -1 \\ \end{pmatrix}$$

**4. Explanation of size requirements**

Matrix addition is defined as an entry-by-entry operation, where each element in the first matrix is added to the corresponding element in the second matrix. If the matrices have different dimensions, they lack a complete one-to-one correspondence between their entries, making the operation undefined.