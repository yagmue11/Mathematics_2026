### Exercise 7. A Line Relative to a Plane

For

$$
L:(x,y,z)=(1,1,0)+t(1,-1,0),\qquad \Pi:x+y+z=2,
$$

determine whether the line intersects the plane at one point, is parallel to it, or lies in it. Explain the role of the dot product of the direction vector and the normal vector.

### Solution

**1. Dot product of direction and normal vectors**

From the given equations, the base point and direction vector of $L$ are

$$
p = (1, 1, 0), \qquad v = (1, -1, 0),
$$

and the normal vector of $\Pi$ is

$$
n = (1, 1, 1).
$$

Computing $n \cdot v$ gives

$$
n \cdot v = (1)(1) + (1)(-1) + (1)(0) = 1 - 1 + 0 = 0.
$$

Because $n \cdot v = 0$, the direction vector $v$ is orthogonal to the normal vector $n$, which means $L$ is parallel to $\Pi$ (either strictly parallel with no common points, or entirely contained in $\Pi$).

**2. Checking whether $L$ lies in $\Pi$**

To distinguish between the two subcases, substitute the base point $p = (1, 1, 0)$ into the equation of $\Pi$:

$$
1 + 1 + 0 = 2.
$$

Since $p$ satisfies $x + y + z = 2$, $p \in \Pi$. For any $t \in \mathbb{R}$,

$$
n \cdot (p + tv) = n \cdot p + t(n \cdot v) = 2 + t(0) = 2.
$$

Therefore, the line $L$ lies entirely in the plane $\Pi$.

**3. Role of $n \cdot v$**

The dot product $n \cdot v$ measures the component of the line's direction along the normal to the plane:

- If $n \cdot v \neq 0$, the line moves across the plane's normal direction and pierces $\Pi$ at a unique point.
- If $n \cdot v = 0$, the line maintains a constant signed distance from $\Pi$, so it either never meets $\Pi$ or lies wholly inside it.