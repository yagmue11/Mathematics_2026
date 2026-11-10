### Exercise 9. Area and the Determinant

The vectors

$$u= \begin{pmatrix} 3 \\ 1 \\ \end{pmatrix},\qquad v= \begin{pmatrix} 1 \\ 4 \\ \end{pmatrix}$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

### Solution

**1. Compute the area using the determinant**

The area of the parallelogram spanned by two vectors in two-dimensional space is the absolute value of the determinant of the matrix formed by using the vectors as its columns. Let $A$ be this matrix:

$$A= \begin{pmatrix} 3 & 1 \\ 1 & 4 \\ \end{pmatrix}$$

First, compute the determinant of $A$:

$$\det A = 3 \cdot 4 - 1 \cdot 1 = 11$$

The area is the absolute value of the determinant:

$$\mathrm{Area} = \vert{}11\vert{} = 11$$

**2. Reverse the order of the vectors**

Let $B$ be the matrix formed by placing $v$ as the first column and $u$ as the second column:

$$B= \begin{pmatrix} 1 & 3 \\ 4 & 1 \\ \end{pmatrix}$$

Compute the determinant of $B$:

$$\det B = 1 \cdot 1 - 3 \cdot 4 = -11$$

**3. Explanation of the changes**

Reversing the order of the vectors is equivalent to swapping the two columns of the matrix. A fundamental property of determinants dictates that swapping two columns (or rows) multiplies the determinant by $-1$. Therefore, the determinant changes sign, from $11$ to $-11$.

The geometric area, however, remains unchanged because it is defined as the absolute value of the determinant. Both $\vert{}11\vert{}$ and $\vert{}-11\vert{}$ yield $11$, reflecting that the physical area of the parallelogram does not depend on the order in which its defining vectors are listed.