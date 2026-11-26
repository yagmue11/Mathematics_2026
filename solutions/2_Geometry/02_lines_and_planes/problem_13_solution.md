### Exercise 13. Closest Point on a Plane

Find the point on the plane $x+2y+2z=4$ closest to $P=(3,0,0)$. Give the distance and check that the segment joining the two points is perpendicular to the plane.

### Solution

**1. Closest point $P'$ on the plane**

The point on $\Pi : x + 2y + 2z = 4$ closest to $P=(3,0,0)$ is the orthogonal projection of $P$ onto $\Pi$. The normal vector of $\Pi$ is $n = (1, 2, 2)$, so the normal line through $P$ is

$$
(x, y, z) = (3, 0, 0) + t(1, 2, 2) = (3 + t, 2t, 2t).
$$

Substituting these coordinates into the plane equation $x + 2y + 2z = 4$ gives

$$
(3 + t) + 2(2t) + 2(2t) = 4 \implies 3 + 9t = 4 \implies 9t = 1 \implies t = \frac{1}{9}.
$$

Substituting $t = \frac{1}{9}$ back into the parametric form yields the closest point:

$$
P' = \left(3 + \frac{1}{9},\; 2\left(\frac{1}{9}\right),\; 2\left(\frac{1}{9}\right)\right) = \left(\frac{28}{9},\; \frac{2}{9},\; \frac{2}{9}\right).
$$

**2. Distance from $P$ to $\Pi$**

The distance is the Euclidean length of $\overrightarrow{PP'}$:

$$
\overrightarrow{PP'} = P' - P = \left(\frac{28}{9} - 3,\; \frac{2}{9} - 0,\; \frac{2}{9} - 0\right) = \left(\frac{1}{9},\; \frac{2}{9},\; \frac{2}{9}\right) = \frac{1}{9}(1, 2, 2).
$$

Its norm is

$$
d(P, \Pi) = \|\overrightarrow{PP'}\| = \frac{1}{9}\sqrt{1^2 + 2^2 + 2^2} = \frac{\sqrt{9}}{9} = \frac{3}{9} = \frac{1}{3}.
$$

*(Checking via the distance formula: $\frac{|1(3) + 2(0) + 2(0) - 4|}{\sqrt{1^2 + 2^2 + 2^2}} = \frac{|-1|}{3} = \frac{1}{3}$.)*

**3. Perpendicularity check**

The segment vector is

$$
\overrightarrow{PP'} = \left(\frac{1}{9},\; \frac{2}{9},\; \frac{2}{9}\right) = \frac{1}{9}n.
$$

Because $\overrightarrow{PP'}$ is a scalar multiple of the plane's normal vector $n = (1, 2, 2)$, the segment $PP'$ is perpendicular to the plane.