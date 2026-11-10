### Exercise 14. A System of Equations and the Determinant

Consider the system $Ax=b$, where

$$A= \begin{pmatrix} 1 & 2 \\ k & 4 \\ \end{pmatrix}.$$

For which values of $k$ does the system have exactly one solution for every $b$? For the remaining value, give an example of a right-hand side $b$ for which the system has infinitely many solutions, and an example for which it has no solution.

### Solution

**1. Find the condition for a unique solution**

A linear system $Ax = b$ has exactly one solution for every vector $b$ if and only if the matrix $A$ is invertible. This occurs precisely when its determinant is non-zero.

First, compute the determinant of $A$:

$$\det A = 1 \cdot 4 - 2 \cdot k = 4 - 2k$$

Set the determinant to be non-zero:

$$4 - 2k \neq 0$$

$$2k \neq 4$$

$$k \neq 2$$

The system has exactly one solution for every $b$ when $k \neq 2$.

**2. Analyze the remaining value**

When $k = 2$, the matrix becomes:

$$A= \begin{pmatrix} 1 & 2 \\ 2 & 4 \\ \end{pmatrix}$$

The determinant is zero, so the system will either have infinitely many solutions or no solution, depending on the vector $b$.

**3. Example with infinitely many solutions**

Choose a vector $b$ such that the second row of the augmented system is a scalar multiple of the first row. For example, choose:

$$b= \begin{pmatrix} 1 \\ 2 \\ \end{pmatrix}$$

The resulting system is:

$$\begin{cases} x + 2y = 1, \\ 2x + 4y = 2. \end{cases}$$

Because the second equation is exactly twice the first equation, it provides no new information. The two equations represent the same line, leaving one free variable. Therefore, the system has infinitely many solutions.

**4. Example with no solution**

Choose a vector $b$ such that the system produces a logical contradiction. For example, choose:

$$b= \begin{pmatrix} 1 \\ 0 \\ \end{pmatrix}$$

The resulting system is:

$$\begin{cases} x + 2y = 1, \\ 2x + 4y = 0. \end{cases}$$

Dividing the second equation by $2$ yields $x + 2y = 0$. This contradicts the first equation, which requires $x + 2y = 1$. Because the two equations represent parallel lines that never intersect, the system has no solution.