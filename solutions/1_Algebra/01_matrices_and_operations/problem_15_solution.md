### Solution

**1. Computation of $(AB)C$**

First, compute the product $AB$:

$$AB = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix}$$

Multiplying the rows by the columns yields:

$$AB = \begin{pmatrix} 1(1) + 2(2) + 0(-1) & 1(0) + 2(1) + 0(3) \\ 0(1) + 1(2) + 1(-1) & 0(0) + 1(1) + 1(3) \\ \end{pmatrix} = \begin{pmatrix} 5 & 2 \\ 1 & 4 \\ \end{pmatrix}$$

Next, compute $(AB)C$ by multiplying this result by $C$:

$$(AB)C = \begin{pmatrix} 5 & 2 \\ 1 & 4 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix}$$

$$(AB)C = \begin{pmatrix} 5(2) + 2(0) & 5(1) + 2(-1) \\ 1(2) + 4(0) & 1(1) + 4(-1) \\ \end{pmatrix} = \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}$$

**2. Computation of $A(BC)$**

First, compute the product $BC$:

$$BC = \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix}$$

Multiplying the rows by the columns yields:

$$BC = \begin{pmatrix} 1(2) + 0(0) & 1(1) + 0(-1) \\ 2(2) + 1(0) & 2(1) + 1(-1) \\ -1(2) + 3(0) & -1(1) + 3(-1) \\ \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \\ \end{pmatrix}$$

Next, compute $A(BC)$ by multiplying $A$ by this result:

$$A(BC) = \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \\ \end{pmatrix}$$

$$A(BC) = \begin{pmatrix} 1(2) + 2(4) + 0(-2) & 1(1) + 2(1) + 0(-4) \\ 0(2) + 1(4) + 1(-2) & 0(1) + 1(1) + 1(-4) \\ \end{pmatrix} = \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}$$

**3. Comparison and Associativity**

Comparing the results, the final matrices are identical:

$$(AB)C = A(BC) = \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}$$

However, the number of scalar multiplications required differs:

* Computing $AB$ requires $12$ multiplications ($4$ entries $\times$ $3$ multiplications), and multiplying by $C$ requires $8$ more ($4$ entries $\times$ $2$ multiplications), for a total of $20$ multiplications.
* Computing $BC$ requires $12$ multiplications ($6$ entries $\times$ $2$ multiplications), and multiplying by $A$ requires $12$ more ($4$ entries $\times$ $3$ multiplications), for a total of $24$ multiplications.

This example illustrates the associativity of matrix multiplication. Associativity means that the way matrices are grouped with parentheses does not change the final product. Geometrically, composing three linear transformations yields the same result regardless of the order in which we combine their matrices. Computationally, however, associativity is highly valuable because it allows us to choose the most efficient grouping (in this case, $(AB)C$) to minimize the total number of arithmetic operations.