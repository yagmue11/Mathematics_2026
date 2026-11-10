### Exercise 15. Combining Determinant Properties

Let $A$ and $B$ be invertible $2\times2$ matrices with

$$\det A=-2,\qquad \det B=3.$$

Without finding the entries of the matrices, compute

$$\det(B^{-1}A^TB).$$

State the determinant properties you use in order and explain why the factors involving $B$ eventually cancel.

### Solution

**1. Expand the determinant of the product**

The determinant is multiplicative, meaning the determinant of a matrix product is the product of their individual determinants:

$$\det(B^{-1}A^TB) = \det(B^{-1}) \cdot \det(A^T) \cdot \det(B)$$

**2. Apply properties for the inverse and transpose**

The determinant of an inverse matrix is the reciprocal of the original matrix's determinant:

$$\det(B^{-1}) = \frac{1}{\det B}$$

The determinant of a transposed matrix is equal to the determinant of the original matrix:

$$\det(A^T) = \det A$$

Substituting these into the expanded product yields:

$$\det(B^{-1}A^TB) = \frac{1}{\det B} \cdot \det A \cdot \det B$$

**3. Compute the final value and explain the cancellation**

Because the determinant maps a matrix to a single scalar number, the resulting expression is a product of real numbers. Since the multiplication of real numbers is commutative, the order of the scalar factors does not matter and can be rearranged:

$$\begin{aligned} \det(B^{-1}A^TB) &= \det A \cdot \left( \frac{1}{\det B} \cdot \det B \right) \\ &= \det A \cdot 1 \\ &= -2 \end{aligned}$$

The factors involving $B$ cancel out because the determinant of the inverse, $\frac{1}{3}$, and the determinant of the original matrix, $3$, are scalar reciprocals that multiply to $1$.