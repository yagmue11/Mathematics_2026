### Exercise 4. Triangular Matrix

Without expanding the determinant, compute

$$\det \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \\ \end{pmatrix}$$

State the rule for an arbitrary triangular matrix and explain it using this example.

### Solution

**1. Compute the determinant**

Because the given matrix is upper triangular, its determinant is the product of its main diagonal entries:

$$\det \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \\ \end{pmatrix} = 2 \cdot (-3) \cdot 7 = -42$$

**2. General rule for an arbitrary triangular matrix**

For any $n \times n$ upper triangular, lower triangular, or diagonal matrix $T = (t_{ij})$, the determinant equals the product of the entries on its main diagonal:

$$\det T = t_{11} t_{22} \cdots t_{nn} = \prod_{i=1}^{n} t_{ii}$$

**3. Explanation using the example**

In the matrix

$$A = \begin{pmatrix} 2 & 4 & 1 \\ 0 & -3 & 5 \\ 0 & 0 & 7 \\ \end{pmatrix}$$

all entries strictly below the main diagonal are zero ($a_{21} = 0$, $a_{31} = 0$, and $a_{32} = 0$).

In the definition of the determinant as a sum over all permutations $\sigma$ of $\{1, 2, 3\}$,

$$\det A = \sum_{\sigma} \mathrm{sgn}(\sigma)\, a_{1,\sigma(1)} a_{2,\sigma(2)} a_{3,\sigma(3)}$$

any permutation that picks an entry below the main diagonal has $\sigma(i) < i$ for at least one row $i$. In our example:

* Choosing from the third row requires $\sigma(3) = 3$, because $a_{31} = 0$ and $a_{32} = 0$.
* Once $\sigma(3) = 3$ is fixed, choosing a non-zero entry from the second row requires $\sigma(2) = 2$, because $a_{21} = 0$.
* Consequently, the first row must use the remaining column $\sigma(1) = 1$.

Thus, the identity permutation $\sigma = (1, 2, 3)$ is the only permutation that produces a non-zero product, leaving only the main diagonal term $a_{11} a_{22} a_{33} = 2 \cdot (-3) \cdot 7 = -42$.