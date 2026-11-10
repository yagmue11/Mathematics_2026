### Exercise 6. A System with a Parameter — Which Cases Actually Occur?

Analyze, depending on the parameter $a$, the system

$$\begin{cases} x+y=2, \\ ax+ay=4. \end{cases}$$

Among the three possibilities — exactly one solution, infinitely many solutions, no solution — determine which actually occur and for which values of $a$. If one type cannot occur, explain why.

### Solution

**1. Form the augmented matrix and reduce**

Extract the coefficients and constant terms into an augmented matrix:

$$\begin{pmatrix} 1 & 1 & \mid & 2 \\ a & a & \mid & 4 \\ \end{pmatrix}$$

Apply a row operation to eliminate the entry below the first pivot. Replace Row 2 with $R_2 - aR_1$:

$$\begin{pmatrix} 1 & 1 & \mid & 2 \\ 0 & 0 & \mid & 4 - 2a \\ \end{pmatrix}$$

**2. Analyze the parameter conditions**

The resulting system corresponding to the reduced matrix is:

$$\begin{cases} x + y = 2, \\ 0 = 4 - 2a. \end{cases}$$

The behavior of the system depends entirely on the value of the parameter $a$ in the second equation.

* **Case 1: No solution**
If $4 - 2a \neq 0$, which means $a \neq 2$, the second equation results in a logical contradiction ($0 = c$, where $c \neq 0$). Therefore, the system has no solution for all $a \neq 2$.
* **Case 2: Infinitely many solutions**
If $4 - 2a = 0$, which means $a = 2$, the second equation becomes $0 = 0$. The system is consistent and reduces to the single equation $x + y = 2$. Because there are two variables and only one pivot, $y$ becomes a free variable. Therefore, the system has infinitely many solutions for $a = 2$.

**3. Explain the impossible case**

The case of **exactly one solution** cannot occur for any value of $a$.

A linear system with two equations and two variables has a unique solution if and only if the determinant of its coefficient matrix is non-zero. The determinant of the coefficient matrix is:

$$\det A = 1(a) - 1(a) = 0$$

Because the determinant is identically zero for all real numbers $a$, the rows of the coefficient matrix are always linearly dependent. Geometrically, the two equations will always represent either parallel lines (when $a \neq 2$) or the exact same line (when $a = 2$). They will never intersect at a single unique point.