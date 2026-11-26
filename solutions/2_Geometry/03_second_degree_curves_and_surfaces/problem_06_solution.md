### Exercise 6. Shifted Ellipse

Reduce

$$
4x^2+9y^2-16x+18y-11=0
$$

to canonical form. Give the center and semiaxis lengths. Check that substituting the coordinates of the center into the left-hand side gives a value consistent with the form you obtained.

### Solution

**1. Completing the square**

Group the $x$-terms and $y$-terms and factor out the leading coefficients:

$$
4(x^2 - 4x) + 9(y^2 + 2y) = 11.
$$

Complete the square inside each parenthesis:

$$
4(x^2 - 4x + 4 - 4) + 9(y^2 + 2y + 1 - 1) = 11,
$$

$$
4(x - 2)^2 - 16 + 9(y + 1)^2 - 9 = 11,
$$

$$
4(x - 2)^2 + 9(y + 1)^2 = 36.
$$

Divide both sides by $36$ to obtain the canonical form:

$$
\frac{(x - 2)^2}{9} + \frac{(y + 1)^2}{4} = 1.
$$

**2. Center and semiaxis lengths**

- **Center:** $(x_0, y_0) = (2, -1)$,
- **Horizontal semiaxis length:** $a = \sqrt{9} = 3$,
- **Vertical semiaxis length:** $b = \sqrt{4} = 2$.

**3. Consistency check at the center**

From the algebraic completion of the square, the left-hand side satisfies the identity

$$
4x^2 + 9y^2 - 16x + 18y - 11 = 4(x - 2)^2 + 9(y + 1)^2 - 36.
$$

Evaluating the original left-hand side at the center $(2, -1)$ gives

$$
4(2)^2 + 9(-1)^2 - 16(2) + 18(-1) - 11 = 16 + 9 - 32 - 18 - 11 = -36,
$$

which matches $4(0)^2 + 9(0)^2 - 36 = -36$ from the completed-square form.