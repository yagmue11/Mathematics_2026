### Exercise 5. Matrix-Vector Product

Let

$$A= \begin{pmatrix} 2 & -1 \\ 1 & 3 \\ \end{pmatrix},\qquad x= \begin{pmatrix} 4 \\ 2 \\ \end{pmatrix}.$$

Compute $Ax$. Then express $Ax$ as a linear combination of the columns of $A$, with coefficients coming from the vector $x$.

### Solution

**1. Computation of $Ax$**

$$Ax = \begin{pmatrix} 2 & -1 \\ 1 & 3 \\ \end{pmatrix} \begin{pmatrix} 4 \\ 2 \\ \end{pmatrix}$$

Multiplying the rows of $A$ by the vector $x$ yields:

$$Ax = \begin{pmatrix} 2(4) + (-1)(2) \\ 1(4) + 3(2) \\ \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \\ \end{pmatrix}$$

**2. Linear Combination of Columns**

The columns of matrix $A$ are the vectors:

$$c_1 = \begin{pmatrix} 2 \\ 1 \\ \end{pmatrix}, \qquad c_2 = \begin{pmatrix} -1 \\ 3 \\ \end{pmatrix}$$

The entries of the vector $x$ serve as the scalar coefficients. Expressing $Ax$ as a linear combination of the columns gives:

$$Ax = 4 \begin{pmatrix} 2 \\ 1 \\ \end{pmatrix} + 2 \begin{pmatrix} -1 \\ 3 \\ \end{pmatrix}$$

Evaluating this sum confirms the previous result:

$$Ax = \begin{pmatrix} 8 \\ 4 \\ \end{pmatrix} + \begin{pmatrix} -2 \\ 6 \\ \end{pmatrix} = \begin{pmatrix} 6 \\ 10 \\ \end{pmatrix}$$