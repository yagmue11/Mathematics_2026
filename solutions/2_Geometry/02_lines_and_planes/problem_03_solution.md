### Exercise 3. Plane Through a Point with a Given Normal Vector

Find the equation of the plane through $P=(1,-2,3)$ and perpendicular to $n=(2,1,-1)$. Check the result by substituting the point $P$ and explain the role of the normal vector.

### Solution

**1. Equation of the plane**

A point $X=(x,y,z)$ lies in the plane through $P=(1,-2,3)$ with normal vector $n=(2,1,-1)$ if and only if the displacement vector $\overrightarrow{PX} = X - P$ is orthogonal to $n$:

$$
n \cdot (X - P) = 0.
$$

Substituting the coordinates gives

$$
2(x - 1) + 1(y + 2) - 1(z - 3) = 0.
$$

Expanding and combining constants yields

$$
2x - 2 + y + 2 - z + 3 = 0,
$$

so the equation of the plane is

$$
2x + y - z + 3 = 0.
$$

**2. Verification**

Substituting $P=(1,-2,3)$ into the equation gives

$$
2(1) + (-2) - 3 + 3 = 0.
$$

The equality holds, confirming that $P$ lies in the plane.

**3. Role of the normal vector**

The normal vector $n=(2,1,-1)$ defines the orientation of the plane in $\mathbb{R}^3$: every displacement vector between two points in the plane must be orthogonal to $n$. In the general equation $ax + by + cz + d = 0$, the components of $n$ directly supply the coefficients $(a,b,c)$, whereas the given point $P$ fixes the constant shift $d$.