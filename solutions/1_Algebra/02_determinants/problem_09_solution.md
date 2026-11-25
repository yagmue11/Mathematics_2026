### Exercise 9. Area and the Determinant

The vectors

$$u= \begin{pmatrix} 3 \\ 1 \\ \end{pmatrix},\qquad v= \begin{pmatrix} 1 \\ 4 \\ \end{pmatrix}$$

span a parallelogram. Compute its area using a determinant. Then reverse the order of the vectors and explain what changes in the determinant and what does not change in the area.

### Solution

**1. Compute the area of the parallelogram**

Form the $2 \times 2$ matrix $A$ whose columns are $u$ and $v$:

$$A = \begin{pmatrix} 3 & 1 \\ 1 & 4 \\ \end{pmatrix}$$

Compute the determinant of $A$:

$$\det A = 3 \cdot 4 - 1 \cdot 1 = 12 - 1 = 11$$

The area of the parallelogram spanned by $u$ and $v$ is the absolute value of this determinant:

$$\mathrm{Area} = \vert{}\det A\vert{} = \vert{}11\vert{} = 11$$

**2. Reverse the order of the vectors**

Form the matrix $B$ by placing $v$ as the first column and $u$ as the second column:

$$B = \begin{pmatrix} 1 & 3 \\ 4 & 1 \\ \end{pmatrix}$$

Compute the determinant of $B$:

$$\det B = 1 \cdot 1 - 3 \cdot 4 = 1 - 12 = -11$$

**3. Comparison of the determinant and the area**

* **What changes in the determinant:** Swapping two columns of a matrix multiplies its determinant by $-1$, so $\det B = -\det A = -11$. Geometrically, reversing the order of the vectors changes the orientation of the ordered pair from counterclockwise $(u, v)$ to clockwise $(v, u)$, which flips the sign of the signed area.
* **What does not change in the area:** Geometric area is non-negative and equals the absolute value of the determinant. Because $\vert{}-11\vert{} = \vert{}11\vert{} = 11$, the area of the parallelogram remains unchanged.