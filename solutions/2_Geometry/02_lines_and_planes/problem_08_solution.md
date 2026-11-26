### Exercise 8. Intersection Point of a Line and a Plane

Find the intersection point of

$$
(x,y,z)=(1,0,2)+t(1,2,-1)
$$

with the plane $x+y+z=4$. Check the result by substituting it into both descriptions.

### Solution

**1. Solving for the parameter $t$**

A general point on the line has coordinates

$$
x = 1 + t, \qquad y = 2t, \qquad z = 2 - t.
$$

Substituting these expressions into the plane equation $x + y + z = 4$ gives

$$
(1 + t) + (2t) + (2 - t) = 4.
$$

Combining like terms yields

$$
2t + 3 = 4 \implies 2t = 1 \implies t = \frac{1}{2}.
$$

**2. Coordinates of the intersection point**

Substituting $t = \frac{1}{2}$ back into the parametric equations of the line gives

$$
(x, y, z) = \left(1 + \frac{1}{2},\; 2\left(\frac{1}{2}\right),\; 2 - \frac{1}{2}\right) = \left(\frac{3}{2},\; 1,\; \frac{3}{2}\right).
$$

The intersection point is $\left(\frac{3}{2}, 1, \frac{3}{2}\right)$.

**3. Verification**

- **In the plane equation:**

$$
\frac{3}{2} + 1 + \frac{3}{2} = 3 + 1 = 4.
$$

- **In the line equation:** for $t = \frac{1}{2}$,

$$
(1, 0, 2) + \frac{1}{2}(1, 2, -1) = \left(1 + \frac{1}{2},\; 0 + 1,\; 2 - \frac{1}{2}\right) = \left(\frac{3}{2},\; 1,\; \frac{3}{2}\right).
$$

Both descriptions are satisfied at $\left(\frac{3}{2}, 1, \frac{3}{2}\right)$.