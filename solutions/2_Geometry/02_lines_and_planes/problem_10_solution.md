### Exercise 10. Projection of a Point onto a Plane

Find the orthogonal projection of $P=(2,1,3)$ onto the plane $x+y+z=3$, and then find the reflection of $P$ across this plane. Check that the midpoint of the segment joining the point and its reflection lies on the plane.

### Solution

**1. Orthogonal projection $P'$ onto the plane**

The plane $\Pi : x + y + z = 3$ has normal vector $n = (1, 1, 1)$. The line passing through $P=(2,1,3)$ perpendicular to $\Pi$ has parametric equation

$$
L : (x, y, z) = (2, 1, 3) + t(1, 1, 1) = (2 + t, 1 + t, 3 + t).
$$

The orthogonal projection $P'$ is the intersection of $L$ with $\Pi$. Substituting the parametric coordinates into $x + y + z = 3$ gives

$$
(2 + t) + (1 + t) + (3 + t) = 3 \implies 6 + 3t = 3 \implies 3t = -3 \implies t = -1.
$$

Substituting $t = -1$ into $L$ yields the orthogonal projection:

$$
P' = (2 - 1, 1 - 1, 3 - 1) = (1, 0, 2).
$$

**2. Reflection $P''$ across the plane**

The projection $P'$ is the midpoint of the segment joining $P$ and its reflection $P''$, so $P' = \frac{1}{2}(P + P'')$, or equivalently,

$$
P'' = 2P' - P = P + 2(P' - P).
$$

Computing $P''$:

$$
P'' = 2(1, 0, 2) - (2, 1, 3) = (2 - 2, 0 - 1, 4 - 3) = (0, -1, 1).
$$

*(Equivalently, $P''$ corresponds to parameter $t = 2(-1) = -2$ along $L$.)*

**3. Midpoint verification**

The midpoint $M$ of the segment $PP''$ is

$$
M = \frac{P + P''}{2} = \left(\frac{2 + 0}{2},\; \frac{1 + (-1)}{2},\; \frac{3 + 1}{2}\right) = (1, 0, 2) = P'.
$$

Substituting $M = (1, 0, 2)$ into the plane equation gives

$$
1 + 0 + 2 = 3,
$$

confirming that the midpoint lies on the plane.