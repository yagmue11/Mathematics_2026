### Exercise 9. A System from a Sum Condition

Find numbers $x,y$ satisfying

$$
x+y=10,\qquad 2x+5y=32.
$$

Solve the system and explain geometrically why the solution is unique.

### Solution

**1. Solve the system**

Set up the augmented matrix for the system:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
2 & 5 & \mid & 32
\end{pmatrix}
$$

Apply a row operation to reach upper triangular form. Replace Row 2 with $R_2 - 2R_1$:

$$
\begin{pmatrix}
1 & 1 & \mid & 10 \\
0 & 3 & \mid & 12
\end{pmatrix}
$$

Translate the matrix back into a system of linear equations using back substitution:

$$
\begin{cases}
x + y = 10, \\
3y = 12.
\end{cases}
$$

From the second equation, solve for $y$:

$$
y = 4
$$

Substitute $y = 4$ into the first equation to solve for $x$:

$$
\begin{aligned}
x + 4 &= 10 \\
x &= 6
\end{aligned}
$$

The unique solution is $x = 6$ and $y = 4$.

**2. Geometric explanation of uniqueness**

Each linear equation in two variables represents a straight line in the Cartesian plane.

- The first equation, $x + y = 10$, corresponds to a line with a slope of $-1$.
- The second equation, $2x + 5y = 32$, can be rewritten in slope-intercept form as $y = -\frac{2}{5}x + \frac{32}{5}$, corresponding to a line with a slope of $-\frac{2}{5}$.

Because the two lines have different slopes, they are non-parallel. In a two-dimensional plane, two distinct non-parallel lines intersect at exactly one unique point, which corresponds to the single coordinate pair $(6, 4)$ satisfying both equations simultaneously.