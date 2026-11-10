### Exercise 5. Row Echelon Form and Number of Solutions

For the augmented matrix

$$\begin{pmatrix} 1 & 2 & -1 & \mid & 3 \\ 0 & 1 & 2 & \mid & 1 \\ 0 & 0 & 0 & \mid & 0 \\ \end{pmatrix}$$

determine the number of solutions and write them in parametric form. Explain how you know how many variables may be chosen freely.

### Solution

**1. Determine the number of solutions and free variables**

The augmented matrix represents a consistent system because the final row ($0 = 0$) does not present a logical contradiction (such as $0 = 1$).

To determine the number of solutions, count the pivot entries (the leading non-zero entries in each row). The matrix has two pivots: the $1$ in the first column and the $1$ in the second column. These correspond to the first two variables, $x$ and $y$.

The third column, which corresponds to the variable $z$, does not contain a pivot. Variables associated with non-pivot columns are free variables. Because the system is consistent and contains at least one free variable, it has infinitely many solutions.

The number of free variables is exactly the total number of unknowns minus the number of pivot columns. Here, $3$ unknowns minus $2$ pivot columns yields $1$ free variable.

**2. Solve using back substitution**

Translate the non-zero rows of the row echelon matrix back into algebraic equations:

$$\begin{cases} x + 2y - z = 3, \\ y + 2z = 1. \end{cases}$$

Assign a parameter to the free variable $z$. Let $z = t$, where $t \in \mathbb{R}$.

Substitute $z = t$ into the second equation to solve for $y$:

$$\begin{aligned} y + 2t &= 1 \\ y &= 1 - 2t \end{aligned}$$

Substitute $y = 1 - 2t$ and $z = t$ into the first equation to solve for $x$:

$$\begin{aligned} x + 2(1 - 2t) - t &= 3 \\ x + 2 - 4t - t &= 3 \\ x + 2 - 5t &= 3 \\ x &= 1 + 5t \end{aligned}$$

**3. Write the solution in parametric form**

The solutions for the variables are:

$$\begin{cases} x = 1 + 5t, \\ y = 1 - 2t, \\ z = t. \end{cases}$$

In vector parametric form, the general solution is expressed as:

$$\begin{pmatrix} x \\ y \\ z \\ \end{pmatrix} = \begin{pmatrix} 1 \\ 1 \\ 0 \\ \end{pmatrix} + t \begin{pmatrix} 5 \\ -2 \\ 1 \\ \end{pmatrix}, \qquad t \in \mathbb{R}$$