### Exercise 4. Gauss–Jordan

Find $A^{-1}$ using the Gauss–Jordan method for

$$
A = \begin{pmatrix}
1 & 2 \\
3 & 5
\end{pmatrix}
$$

Show the augmented matrix $[A\mid I]$ after successive operations and explain why obtaining $I$ on the left gives the inverse on the right.

### Solution

**1. Form the initial augmented matrix**

Set up the augmented matrix $[A \mid I]$:

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
3 & 5 & \mid & 0 & 1
\end{pmatrix}
$$

**2. Apply row operations to reach $[I \mid A^{-1}]$**

- **Step 1:** Replace Row 2 with $R_2 - 3R_1$.

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & -1 & \mid & -3 & 1
\end{pmatrix}
$$

- **Step 2:** Multiply Row 2 by $-1$.

$$
\begin{pmatrix}
1 & 2 & \mid & 1 & 0 \\
0 & 1 & \mid & 3 & -1
\end{pmatrix}
$$

- **Step 3:** Replace Row 1 with $R_1 - 2R_2$.

$$
\begin{pmatrix}
1 & 0 & \mid & -5 & 2 \\
0 & 1 & \mid & 3 & -1
\end{pmatrix}
$$

**3. State the inverse matrix**

The matrix on the right side of the augmented system is $A^{-1}$:

$$
A^{-1} = \begin{pmatrix}
-5 & 2 \\
3 & -1
\end{pmatrix}
$$

**4. Explain why the method works**

Each elementary row operation corresponds to multiplying the augmented matrix from the left by an invertible elementary matrix $E_i$. Performing a sequence of row operations $E_1, E_2, \dots, E_k$ transforms the system as follows:

$$
(E_k \cdots E_2 E_1) [A \mid I] = [(E_k \cdots E_2 E_1)A \mid (E_k \cdots E_2 E_1)I]
$$

When the left side is transformed into the identity matrix $I$, the net operation matrix $M = E_k \cdots E_2 E_1$ satisfies $MA = I$, which means $M = A^{-1}$.

Applying that same transformation matrix $M$ to $I$ on the right side produces:

$$
MI = A^{-1}I = A^{-1}
$$

Thus, once the left block reaches $I$, the right block contains $A^{-1}$.