### Exercise 8. Sphere

Reduce

$$
x^2+y^2+z^2-4x+2y-6z-2=0
$$

to canonical form. Find the center and radius. Give two points on the sphere and check them in the equation.

### Solution

**1. Completing the square**

Group terms by variable and move the constant to the right-hand side:

$$
(x^2 - 4x) + (y^2 + 2y) + (z^2 - 6z) = 2.
$$

Complete the square for $x$, $y$, and $z$ by adding $4$, $1$, and $9$ to both sides:

$$
(x^2 - 4x + 4) + (y^2 + 2y + 1) + (z^2 - 6z + 9) = 2 + 4 + 1 + 9,
$$

which gives the canonical form of the sphere:

$$
(x - 2)^2 + (y + 1)^2 + (z - 3)^2 = 16.
$$

**2. Center and radius**

- **Center:** $C = (2, -1, 3)$,
- **Radius:** $r = \sqrt{16} = 4$.

**3. Two points on the sphere and verification**

Shifting from the center $C = (2, -1, 3)$ by $r = 4$ along the $x$-axis gives two points on the sphere:

$$
P_1 = (2 + 4, -1, 3) = (6, -1, 3), \qquad P_2 = (2 - 4, -1, 3) = (-2, -1, 3).
$$

- **Verification for $P_1 = (6, -1, 3)$:**

$$
6^2 + (-1)^2 + 3^2 - 4(6) + 2(-1) - 6(3) - 2 = 36 + 1 + 9 - 24 - 2 - 18 - 2 = 0.
$$

- **Verification for $P_2 = (-2, -1, 3)$:**

$$
(-2)^2 + (-1)^2 + 3^2 - 4(-2) + 2(-1) - 6(3) - 2 = 4 + 1 + 9 + 8 - 2 - 18 - 2 = 0.
$$

Both points satisfy the original equation.