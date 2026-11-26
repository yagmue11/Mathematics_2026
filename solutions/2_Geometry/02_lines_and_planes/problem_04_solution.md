### Exercise 4. Plane Through Three Points

Find the equation of the plane through

$$
A=(1,0,0),\quad B=(0,1,0),\quad C=(0,0,1).
$$

First construct two vectors lying in the plane, and then use the cross product. Check the resulting equation on all three points.

### Solution

**1. Two vectors in the plane**

Using $A=(1,0,0)$ as the reference point, two displacement vectors lying in the plane are

$$
u = \overrightarrow{AB} = B - A = (0 - 1, 1 - 0, 0 - 0) = (-1, 1, 0),
$$

$$
v = \overrightarrow{AC} = C - A = (0 - 1, 0 - 0, 1 - 0) = (-1, 0, 1).
$$

Since $u$ and $v$ are not scalar multiples of each other, they are linearly independent and span the plane.

**2. Normal vector via the cross product**

A normal vector $n$ to the plane is given by the cross product $n = u \times v$:

$$
\begin{aligned}
n &= (-1, 1, 0) \times (-1, 0, 1) \\
  &= (1 \cdot 1 - 0 \cdot 0,\; 0 \cdot (-1) - (-1) \cdot 1,\; (-1) \cdot 0 - 1 \cdot (-1)) \\
  &= (1, 1, 1).
\end{aligned}
$$

**3. Equation of the plane**

Using the normal vector $n=(1,1,1)$ and the point $A=(1,0,0)$ in $n \cdot (X - A) = 0$ gives

$$
1(x - 1) + 1(y - 0) + 1(z - 0) = 0,
$$

which simplifies to

$$
x + y + z = 1.
$$

**4. Verification on all three points**

- For $A=(1,0,0)$: $1 + 0 + 0 = 1$.
- For $B=(0,1,0)$: $0 + 1 + 0 = 1$.
- For $C=(0,0,1)$: $0 + 0 + 1 = 1$.

All three points satisfy $x + y + z = 1$.