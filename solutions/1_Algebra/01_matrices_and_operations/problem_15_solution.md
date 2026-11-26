### Exercise 15. Associativity of Multiplication and Different Calculation Paths

Given

$$A= \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix},\quad B= \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix},\quad C= \begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix}.$$

Compute $(AB)C$ and $A(BC)$. Compare the results and the number of intermediate operations. Explain what associativity of matrix multiplication means in this example.

---

### Solution

**1. Matrix dimensions**

The given matrices have dimensions:

* $A$ is $2 \times 3$,
* $B$ is $3 \times 2$,
* $C$ is $2 \times 2$.

Both products $(AB)C$ and $A(BC)$ are defined and yield a $2 \times 2$ matrix.

**2. Compute $(AB)C$**

First, compute the product $AB$ ($2 \times 3$ multiplied by $3 \times 2$, resulting in a $2 \times 2$ matrix):

$$\begin{aligned} AB &= \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix} \\ &= \begin{pmatrix} 1\cdot 1 + 2\cdot 2 + 0\cdot (-1) & 1\cdot 0 + 2\cdot 1 + 0\cdot 3 \\ 0\cdot 1 + 1\cdot 2 + 1\cdot (-1) & 0\cdot 0 + 1\cdot 1 + 1\cdot 3 \\ \end{pmatrix} \\ &= \begin{pmatrix} 5 & 2 \\ 1 & 4 \\ \end{pmatrix}. \end{aligned}$$

Next, multiply the result on the right by $C$ ($2 \times 2$ multiplied by $2 \times 2$):

$$\begin{aligned} (AB)C &= \begin{pmatrix} 5 & 2 \\ 1 & 4 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix} \\ &= \begin{pmatrix} 5\cdot 2 + 2\cdot 0 & 5\cdot 1 + 2\cdot (-1) \\ 1\cdot 2 + 4\cdot 0 & 1\cdot 1 + 4\cdot (-1) \\ \end{pmatrix} \\ &= \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}. \end{aligned}$$

**3. Compute $A(BC)$**

First, compute the product $BC$ ($3 \times 2$ multiplied by $2 \times 2$, resulting in a $3 \times 2$ matrix):

$$\begin{aligned} BC &= \begin{pmatrix} 1 & 0 \\ 2 & 1 \\ -1 & 3 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & -1 \\ \end{pmatrix} \\ &= \begin{pmatrix} 1\cdot 2 + 0\cdot 0 & 1\cdot 1 + 0\cdot (-1) \\ 2\cdot 2 + 1\cdot 0 & 2\cdot 1 + 1\cdot (-1) \\ (-1)\cdot 2 + 3\cdot 0 & (-1)\cdot 1 + 3\cdot (-1) \\ \end{pmatrix} \\ &= \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \\ \end{pmatrix}. \end{aligned}$$

Next, multiply $A$ on the right by $BC$ ($2 \times 3$ multiplied by $3 \times 2$):

$$\begin{aligned} A(BC) &= \begin{pmatrix} 1 & 2 & 0 \\ 0 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 4 & 1 \\ -2 & -4 \\ \end{pmatrix} \\ &= \begin{pmatrix} 1\cdot 2 + 2\cdot 4 + 0\cdot (-2) & 1\cdot 1 + 2\cdot 1 + 0\cdot (-4) \\ 0\cdot 2 + 1\cdot 4 + 1\cdot (-2) & 0\cdot 1 + 1\cdot 1 + 1\cdot (-4) \\ \end{pmatrix} \\ &= \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}. \end{aligned}$$

**4. Comparison of results and intermediate operations**

The final matrices are identical:

$$(AB)C = A(BC) = \begin{pmatrix} 10 & 3 \\ 2 & -3 \\ \end{pmatrix}.$$

Multiplying an $m \times n$ matrix by an $n \times p$ matrix requires $m \cdot n \cdot p$ scalar multiplications and $m \cdot (n - 1) \cdot p$ scalar additions.

| Calculation path | Step 1 operations | Step 2 operations | Total scalar operations |
| --- | --- | --- | --- |
| $(AB)C$ | $AB$ ($2 \times 3 \times 2$): $12$ mult., $8$ add. | $(AB)C$ ($2 \times 2 \times 2$): $8$ mult., $4$ add. | $20$ multiplications, $12$ additions ($32$ total) |
| $A(BC)$ | $BC$ ($3 \times 2 \times 2$): $12$ mult., $6$ add. | $A(BC)$ ($2 \times 3 \times 2$): $12$ mult., $8$ add. | $24$ multiplications, $14$ additions ($38$ total) |

Computing $(AB)C$ requires $4$ fewer scalar multiplications and $2$ fewer scalar additions than computing $A(BC)$ because the intermediate matrix $AB$ ($2 \times 2$) is smaller than $BC$ ($3 \times 2$).

**5. Meaning of associativity in this example**

Associativity of matrix multiplication states that $(AB)C = A(BC)$ whenever the adjacent matrix dimensions match. In this example:

* **Order of factors:** The left-to-right sequence of matrices $A$, $B$, $C$ remains fixed (matrix multiplication is not commutative, so factors cannot be swapped).
* **Freedom of grouping:** Parentheses may be placed freely to group adjacent pairs without changing the final $2 \times 2$ matrix.
* **Computational optimization:** Because the result is independent of parenthesization, one can choose the grouping that minimizes intermediate matrix sizes and total arithmetic operations—here, evaluating $(AB)C$ instead of $A(BC)$.