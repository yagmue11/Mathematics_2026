### Exercise 7. Choosing a Method Deliberately

Do not solve all of the following systems completely. For each situation, choose the method that best uses its structure and justify your choice:

1. one system with a triangular coefficient matrix

$$\begin{cases} 2x-y=3, \\ 4y=8; \end{cases}$$

2. three systems $Ax=b_i$ with the same invertible matrix $A$, when $A^{-1}$ is already known;
3. one $3\times3$ system for which the inverse matrix is not given and the goal is only to find one solution vector.

For case 1, carry out the chosen method completely. For cases 2 and 3, describe the plan and indicate which part of the computation would be reusable or unnecessary. Do not judge a method by its name alone — refer to the number of right-hand sides and the structure of the matrix.

### Solution

**1. A system with a triangular coefficient matrix**

* **Chosen method:** Back substitution.
* **Justification:** The coefficient matrix is already in upper triangular form. Because the variable $x$ has already been eliminated from the second equation, performing Gaussian elimination or computing an inverse matrix would introduce unnecessary steps.
* **Execution:**

From the second equation, solve directly for $y$:

$$4y = 8$$

$$y = 2$$

Substitute $y = 2$ into the first equation to find $x$:

$$\begin{aligned} 2x - 2 &= 3 \\ 2x &= 5 \\ x &= \frac{5}{2} \end{aligned}$$

The solution is the vector:

$$\begin{pmatrix} x \\ y \\ \end{pmatrix} = \begin{pmatrix} \frac{5}{2} \\ 2 \\ \end{pmatrix}$$

**2. Three systems $Ax=b_i$ with a known inverse $A^{-1}$**

* **Chosen method:** Matrix-vector multiplication using $x_i = A^{-1}b_i$.
* **Justification:** Because multiple systems share the exact same coefficient matrix $A$, the transformation required to isolate the variables is identical across all three problems. Since $A^{-1}$ is already given, the system is fundamentally pre-solved.
* **Plan and efficiency:** The plan is to compute three independent matrix-vector products: $A^{-1}b_1$, $A^{-1}b_2$, and $A^{-1}b_3$. The matrix $A^{-1}$ acts as a completely reusable operator. Performing Gaussian elimination from scratch for each right-hand side $b_i$ would be highly inefficient and structurally unnecessary.

**3. One $3\times3$ system to find one solution vector**

* **Chosen method:** Gaussian elimination on the augmented matrix $[A \mid b]$.
* **Justification:** The goal is to evaluate exactly one right-hand side $b$. Finding the inverse matrix $A^{-1}$ from scratch requires row-reducing the augmented matrix $[A \mid I]$, which is equivalent to solving three separate linear systems simultaneously.
* **Plan and efficiency:** The plan is to construct the single augmented matrix $[A \mid b]$, apply row operations to reach upper triangular form, and use back substitution to find the unique solution vector. Because there are no subsequent right-hand sides to evaluate, computing the full inverse matrix $A^{-1}$ is an unnecessary over-computation that requires significantly more arithmetic operations than solving the single specific system directly.