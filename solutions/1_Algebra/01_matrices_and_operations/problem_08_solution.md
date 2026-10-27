### Solution

**1. Row Operations**

The initial matrix is:

$$\begin{pmatrix} 1 & 2 & -1 \\ 2 & 4 & 1 \\ -1 & 1 & 3 \\ \end{pmatrix}$$

**Step 1:** Apply $R_2 \leftarrow R_2 - 2R_1$.

We subtract $2$ times the first row from the second row. The first and third rows remain unchanged.

$$\begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ -1 & 1 & 3 \\ \end{pmatrix}$$

**Step 2:** Apply $R_3 \leftarrow R_3 + R_1$.

We add the first row to the third row.

$$\begin{pmatrix} 1 & 2 & -1 \\ 0 & 0 & 3 \\ 0 & 3 & 2 \\ \end{pmatrix}$$

**Step 3:** Interchange $R_2$ and $R_3$.

We swap the second and third rows, which brings the matrix into an upper triangular form.

$$\begin{pmatrix} 1 & 2 & -1 \\ 0 & 3 & 2 \\ 0 & 0 & 3 \\ \end{pmatrix}$$

**2. Reversing the Operations**

Elementary row operations are fully reversible. The operations that undo the given steps are:

* To reverse $R_2 \leftarrow R_2 - 2R_1$, add $2$ times the first row back to the second row:
$R_2 \leftarrow R_2 + 2R_1$
* To reverse $R_3 \leftarrow R_3 + R_1$, subtract the first row from the third row:
$R_3 \leftarrow R_3 - R_1$
* To reverse the interchange of $R_2$ and $R_3$, simply interchange them again:
Interchange $R_2$ and $R_3$