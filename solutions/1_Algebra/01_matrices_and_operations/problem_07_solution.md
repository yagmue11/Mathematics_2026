### Exercise 7. Matrix Powers and Identities

For

$$A= \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix}$$

compute

$$AI,\qquad IA,\qquad A+0,\qquad A^2,\qquad A^3.$$

Explain the roles of the matrices $I$ and $0$, and describe the pattern you observe in successive powers of $A$.

### Solution

**1. Computations involving the Identity and Zero Matrices**

The identity matrix $I$ and zero matrix $0$ of size $2 \times 2$ are:

$$I = \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix}, \qquad 0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \\ \end{pmatrix}$$

Computing the products and sum yields:

$$AI = \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix}$$

$$IA = \begin{pmatrix} 1 & 0 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix}$$

$$A+0 = \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix} + \begin{pmatrix} 0 & 0 \\ 0 & 0 \\ \end{pmatrix} = \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix}$$

**2. Roles of $I$ and $0$**

The matrix $I$ serves as the multiplicative identity in matrix algebra, analogous to the number $1$ in scalar multiplication; multiplying a square matrix by $I$ (from either side) leaves the matrix unchanged. The matrix $0$ serves as the additive identity, analogous to the number $0$; adding the zero matrix to another matrix of the same size leaves it unchanged.

**3. Computation of Powers**

Multiplying $A$ by itself yields:

$$A^2 = A A = \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix} = \begin{pmatrix} 4 & 4 \\ 0 & 4 \\ \end{pmatrix}$$

Multiplying $A^2$ by $A$ yields:

$$A^3 = A^2 A = \begin{pmatrix} 4 & 4 \\ 0 & 4 \\ \end{pmatrix} \begin{pmatrix} 2 & 1 \\ 0 & 2 \\ \end{pmatrix} = \begin{pmatrix} 8 & 12 \\ 0 & 8 \\ \end{pmatrix}$$

**4. Observed Pattern**

By examining $A^1$, $A^2$, and $A^3$, a clear pattern emerges for the entries of $A^n$:

* The main diagonal entries are the corresponding powers of $2$ (which is $2^n$).
* The bottom-left entry remains constantly $0$.
* The top-right entry follows the pattern $n \cdot 2^{n-1}$.