### Exercise 10. Column-by-Column Matrix Product

Given

$$A= \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix},\qquad B= \begin{pmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \\ \end{pmatrix}.$$

Denote the columns of $B$ by $b_1,b_2$.

1. Compute $Ab_1$ and $Ab_2$.
2. Compute the matrix $AB$.
3. Compare the results and explain why the columns of $AB$ are exactly the vectors $Ab_1$ and $Ab_2$.

### Solution

**1. Computation of $Ab_1$ and $Ab_2$**

The columns of matrix $B$ are the vectors:

$$b_1 = \begin{pmatrix} 1 \\ -1 \\ 3 \\ \end{pmatrix}, \qquad b_2 = \begin{pmatrix} 2 \\ 0 \\ 1 \\ \end{pmatrix}$$

Multiplying matrix $A$ by the first column $b_1$ yields:

$$Ab_1 = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 \\ -1 \\ 3 \\ \end{pmatrix}$$

$$Ab_1 = \begin{pmatrix} 1(1) + 2(-1) + 0(3) \\ 0(1) + 1(-1) + 1(3) \\ \end{pmatrix} = \begin{pmatrix} -1 \\ 2 \\ \end{pmatrix}$$

Multiplying matrix $A$ by the second column $b_2$ yields:

$$Ab_2 = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 2 \\ 0 \\ 1 \\ \end{pmatrix}$$

$$Ab_2 = \begin{pmatrix} 1(2) + 2(0) + 0(1) \\ 0(2) + 1(0) + 1(1) \\ \end{pmatrix} = \begin{pmatrix} 2 \\ 1 \\ \end{pmatrix}$$

**2. Computation of $AB$**

Now, multiply the full matrices $A$ and $B$:

$$AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 2 \\ -1 & 0 \\ 3 & 1 \\ \end{pmatrix}$$

$$AB = \begin{pmatrix} 1(1) + 2(-1) + 0(3) & 1(2) + 2(0) + 0(1) \\ 0(1) + 1(-1) + 1(3) & 0(2) + 1(0) + 1(1) \\ \end{pmatrix}$$

$$AB = \begin{pmatrix} -1 & 2 \\ 2 & 1 \\ \end{pmatrix}$$

**3. Comparison and Explanation**

Comparing the results, the first column of the matrix $AB$ is exactly the vector $Ab_1$, and the second column of $AB$ is exactly the vector $Ab_2$.

This demonstrates a fundamental property of matrix multiplication: the product $AB$ can be computed column by column. The $j$-th column of the resulting matrix $AB$ is strictly determined by multiplying the entire left matrix $A$ by the $j$-th column of the right matrix $B$. This relationship can be expressed block-wise as:

$$AB = \begin{pmatrix} Ab_1 & \mid & Ab_2 \\ \end{pmatrix}$$