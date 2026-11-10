### Exercise 12. Finding Inverses Without Starting from Scratch

It is known that

$$A^{-1}= \begin{pmatrix} 2 & -1 \\ -3 & 2 \\ \end{pmatrix}.$$

Without finding $A$, compute $(3A)^{-1}$, $(A^T)^{-1}$, and $(A^2)^{-1}$. Justify each result using the appropriate property.

### Solution

**1. Compute $(3A)^{-1}$**

The inverse of a scalar multiple of a matrix satisfies the property $(cA)^{-1} = \frac{1}{c}A^{-1}$. Applying this with $c = 3$ yields:

$$\begin{aligned} (3A)^{-1} &= \frac{1}{3} A^{-1} \\ &= \frac{1}{3} \begin{pmatrix} 2 & -1 \\ -3 & 2 \\ \end{pmatrix} \\ &= \begin{pmatrix} \frac{2}{3} & -\frac{1}{3} \\ -1 & \frac{2}{3} \\ \end{pmatrix} \end{aligned}$$

**2. Compute $(A^T)^{-1}$**

The inverse of a transposed matrix is equal to the transpose of its inverse. This property is stated as $(A^T)^{-1} = (A^{-1})^T$.

$$\begin{aligned} (A^T)^{-1} &= (A^{-1})^T \\ &= \begin{pmatrix} 2 & -1 \\ -3 & 2 \\ \end{pmatrix}^T \\ &= \begin{pmatrix} 2 & -3 \\ -1 & 2 \\ \end{pmatrix} \end{aligned}$$

**3. Compute $(A^2)^{-1}$**

The inverse of a matrix product is the product of the inverses in reverse order: $(AB)^{-1} = B^{-1}A^{-1}$. For a matrix squared, this simplifies to $(A^2)^{-1} = (AA)^{-1} = A^{-1}A^{-1} = (A^{-1})^2$.

$$\begin{aligned} (A^2)^{-1} &= (A^{-1})^2 \\ &= \begin{pmatrix} 2 & -1 \\ -3 & 2 \\ \end{pmatrix} \begin{pmatrix} 2 & -1 \\ -3 & 2 \\ \end{pmatrix} \\ &= \begin{pmatrix} 2(2) + (-1)(-3) & 2(-1) + (-1)(2) \\ -3(2) + 2(-3) & -3(-1) + 2(2) \\ \end{pmatrix} \\ &= \begin{pmatrix} 4 + 3 & -2 - 2 \\ -6 - 6 & 3 + 4 \\ \end{pmatrix} \\ &= \begin{pmatrix} 7 & -4 \\ -12 & 7 \\ \end{pmatrix} \end{aligned}$$