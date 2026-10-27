### Solution

**1. Computation of Powers**

First, compute $A^2$:

$$A^2 = A A = \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix}$$

Next, compute $A^3$:

$$A^3 = A^2 A = \begin{pmatrix} 1 & 2 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 1 & 3 \\ 0 & 1 \\ \end{pmatrix}$$

Next, compute $A^4$:

$$A^4 = A^3 A = \begin{pmatrix} 1 & 3 \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix} = \begin{pmatrix} 1 & 4 \\ 0 & 1 \\ \end{pmatrix}$$

**2. Conjecture for $A^n$**

Based on the pattern of the first four powers, the main diagonal entries remain constantly $1$, the bottom-left entry remains $0$, and the top-right entry perfectly matches the exponent. Thus, we conjecture that for any positive integer $n$:

$$A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \\ \end{pmatrix}$$

**3. Verification via Mathematical Induction**

To prove this conjecture, we use mathematical induction. We already know the formula holds for small values of $n$. Now, assume that the formula is true for an arbitrary integer $n$:

$$A^n = \begin{pmatrix} 1 & n \\ 0 & 1 \\ \end{pmatrix}$$

We must show that this assumption implies the formula is also true for $n+1$. To find $A^{n+1}$, we multiply $A^n$ by $A$:

$$A^{n+1} = A^n A = \begin{pmatrix} 1 & n \\ 0 & 1 \\ \end{pmatrix} \begin{pmatrix} 1 & 1 \\ 0 & 1 \\ \end{pmatrix}$$

Multiplying the rows by the columns yields:

$$A^{n+1} = \begin{pmatrix} 1(1) + n(0) & 1(1) + n(1) \\ 0(1) + 1(0) & 0(1) + 1(1) \\ \end{pmatrix}$$

Simplifying the matrix entries produces:

$$A^{n+1} = \begin{pmatrix} 1 & n+1 \\ 0 & 1 \\ \end{pmatrix}$$

This resulting matrix is exactly the proposed formula evaluated at $n+1$. Because assuming the formula works for step $n$ inherently forces it to work for step $n+1$, the conjecture is proven true for all positive integers.