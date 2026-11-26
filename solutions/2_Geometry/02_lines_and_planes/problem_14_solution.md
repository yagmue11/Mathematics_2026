### Exercise 14. Contrast: Intersection and Parallelism

From the point $P=(0,0,1)$, two lines are drawn with direction vectors

$$
v_1=(2,1,-1),\qquad v_2=(2,1,0).
$$

For each line, analyze its position relative to the plane $z=0$.

For the line that intersects the plane, find the intersection point. For the other line, explain how you can recognize parallelism without solving an equation.

### Solution

**1. Setup**

The plane $\Pi : z = 0$ (the $xy$-plane) has normal vector

$$
n = (0, 0, 1).
$$

The two lines through $P = (0, 0, 1)$ are

$$
L_1 : (x, y, z) = (0, 0, 1) + t(2, 1, -1) = (2t, t, 1 - t),
$$

$$
L_2 : (x, y, z) = (0, 0, 1) + s(2, 1, 0) = (2s, s, 1).
$$

**2. Analysis of $L_1$**

The dot product of $v_1$ and $n$ is

$$
n \cdot v_1 = (0, 0, 1) \cdot (2, 1, -1) = -1 \neq 0.
$$

Hence $L_1$ is not parallel to $\Pi$ and intersects it at a single point. Setting $z = 0$ in $L_1$ gives

$$
1 - t = 0 \implies t = 1.
$$

Substituting $t = 1$ into $L_1$ yields the intersection point

$$
(2(1), 1, 1 - 1) = (2, 1, 0).
$$

**3. Analysis of $L_2$**

For $L_2$, the dot product with the normal vector is

$$
n \cdot v_2 = (0, 0, 1) \cdot (2, 1, 0) = 0.
$$

Since $P = (0, 0, 1)$ has $z = 1 \neq 0$, $P$ does not lie in $\Pi$, so $L_2$ is strictly parallel to the plane $z = 0$ and has no intersection points with it.

**4. Recognizing parallelism without solving an equation**

The plane $z = 0$ consists of all points at height $z = 0$, so its normal points purely along the $z$-axis. The direction vector $v_2 = (2, 1, 0)$ has third component $0$, meaning motion along $L_2$ changes only the $x$- and $y$-coordinates while keeping the $z$-coordinate constant at $z = 1$. A line confined to the horizontal level $z = 1$ is automatically parallel to the horizontal plane $z = 0$.