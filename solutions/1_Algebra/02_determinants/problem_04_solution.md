### Exercise 4. Triangular Matrix

Without expanding the determinant, compute

$$\det \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \\ \end{pmatrix}.$$

State the rule for an arbitrary triangular matrix and explain it using this example.


### Solution

**1. Compute the determinant**

$$\det \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \\ \end{pmatrix} = 2 \cdot (-3) \cdot 7 = -42$$

**2. State the rule**

The determinant of any upper triangular, lower triangular, or diagonal matrix is equal to the product of the entries on its main diagonal.

**3. Explain the rule using the example**

If one were to compute the determinant using cofactor expansion along the first column, the only non-zero term is the one corresponding to the first entry, $2$:

$$\det \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \\ \end{pmatrix} = 2 \cdot \det \begin{pmatrix} -3 & 5 \\ 0 & 7 \\ \end{pmatrix}$$

Continuing the expansion along the first column of the resulting $2 \times 2$ matrix, the only non-zero term corresponds to the entry $-3$:

$$2 \cdot ( -3 \cdot 7 - 5 \cdot 0 ) = 2 \cdot (-3) \cdot 7 = -42$$

The zeroes below the main diagonal force all other cofactors in a first-column expansion to be multiplied by zero, leaving only the product of the diagonal entries.