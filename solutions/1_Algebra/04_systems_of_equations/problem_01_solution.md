### Exercise 1. From a System to a Matrix

Write the system

$$\begin{cases} 2x-y+z=4, \\ x+3y-2z=1, \\ 3x+y+z=7. \end{cases}$$

in the form $Ax=b$.
Identify the coefficient matrix, the vector of unknowns, and the right-hand side vector. Explain how each row of the matrix corresponds to one equation.

### Solution

**1. Identify the components**

The linear system can be separated into the coefficients multiplying the variables, the variables themselves, and the constant terms on the right side of the equations.

The coefficient matrix $A$ contains the numerical multipliers from the left side of the system, ordered by variable ($x$, $y$, $z$) in each column:

$$A= \begin{pmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \\ \end{pmatrix}$$

The vector of unknowns $x$ contains the variables of the system as a column vector:

$$x= \begin{pmatrix} x \\ y \\ z \\ \end{pmatrix}$$

The right-hand side vector $b$ contains the constants from the right side of the equals signs:

$$b= \begin{pmatrix} 4 \\ 1 \\ 7 \\ \end{pmatrix}$$

**2. Write the system in $Ax=b$ form**

Substituting the identified components into the matrix equation $Ax = b$ yields:

$$\begin{pmatrix} 2 & -1 & 1 \\ 1 & 3 & -2 \\ 3 & 1 & 1 \\ \end{pmatrix} \begin{pmatrix} x \\ y \\ z \\ \end{pmatrix} = \begin{pmatrix} 4 \\ 1 \\ 7 \\ \end{pmatrix}$$

**3. Explanation of row correspondence**

By the definition of matrix-vector multiplication, multiplying the matrix $A$ by the vector $x$ involves taking the dot product of each row of $A$ with the column vector $x$.

For the first row, this operation pairs the elements of the row with the variables: $2(x) + (-1)(y) + 1(z)$. Setting this product equal to the corresponding first entry of the vector $b$ reconstructs the first equation of the system:

$$2x - y + z = 4$$

This exact pattern applies to every row. Each horizontal row of the coefficient matrix represents the left-hand side of a single linear equation, while the corresponding entry in the vector $b$ provides the value that the equation must equal.