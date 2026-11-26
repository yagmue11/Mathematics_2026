### Exercise 13. Intersection of a Sphere and a Plane

Given the sphere

$$
x^2+y^2+z^2=25
$$

and the plane $z=3$, find the equation of the intersection curve and its radius. Then describe what happens for $z=c$ depending on $c$.

### Solution

**1. Intersection with the plane $z = 3$**

Substituting $z = 3$ into the sphere equation $x^2 + y^2 + z^2 = 25$ gives

$$
x^2 + y^2 + 3^2 = 25 \implies x^2 + y^2 = 16.
$$

The intersection curve is a **circle** in the plane $z = 3$ described by

$$
\begin{cases}
x^2 + y^2 = 16, \\
z = 3,
\end{cases}
$$

centered at $(0, 0, 3)$ with radius

$$
r = \sqrt{16} = 4.
$$

**2. Behavior of the cross-section $z = c$ depending on $c$**

For an arbitrary horizontal plane $z = c$, substituting $z = c$ yields

$$
x^2 + y^2 = 25 - c^2.
$$

There are three cases depending on the value of $c$:

- **$|c| < 5$ ($-5 < c < 5$):** Here $25 - c^2 > 0$, so the plane intersects the sphere in a **circle** centered at $(0, 0, c)$ with radius $r(c) = \sqrt{25 - c^2}$. The radius reaches its maximum $r(0) = 5$ at the equator $c = 0$ and decreases toward $0$ as $|c| \to 5$.
- **$|c| = 5$ ($c = 5$ or $c = -5$):** Here $25 - c^2 = 0$, so the plane is tangent to the sphere and intersects it at a **single point**—the north pole $(0, 0, 5)$ or the south pole $(0, 0, -5)$.
- **$|c| > 5$:** Here $25 - c^2 < 0$, so the equation $x^2 + y^2 = 25 - c^2$ has no real solutions and the **intersection is empty**.