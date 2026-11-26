### Exercise 11. Plane Containing a Line and a Point

Find the equation of the plane containing

$$
(x,y,z)=(1,0,2)+t(1,1,-1)
$$

and the point $P=(0,2,1)$. Check that both the entire line and the point lie in the plane you obtain.

### Solution

**1. Two linearly independent direction vectors in the plane**

The given line $L$ passes through $A = (1, 0, 2)$ with direction vector

$$
v = (1, 1, -1).
$$

First verify that $P = (0, 2, 1)$ does not lie on $L$: the first coordinate requires $1 + t = 0 \implies t = -1$, which yields $(0, -1, 3) \neq (0, 2, 1)$. Thus $P \notin L$, and a second direction vector in the plane is

$$
u = \overrightarrow{AP} = P - A = (0 - 1, 2 - 0, 1 - 2) = (-1, 2, -1).
$$

**2. Normal vector and plane equation**

A normal vector $n$ to the plane is obtained from the cross product $n = v \times u$:

$$
\begin{aligned}
n &= (1, 1, -1) \times (-1, 2, -1) \\
  &= (1(-1) - (-1)(2),\; (-1)(-1) - 1(-1),\; 1(2) - 1(-1)) \\
  &= (-1 + 2,\; 1 + 1,\; 2 + 1) \\
  &= (1, 2, 3).
\end{aligned}
$$

Using $n = (1, 2, 3)$ and the point $A = (1, 0, 2)$ in $n \cdot (X - A) = 0$ gives

$$
1(x - 1) + 2(y - 0) + 3(z - 2) = 0,
$$

which simplifies to

$$
x + 2y + 3z = 7.
$$

**3. Verification**

- **For the point $P = (0, 2, 1)$:**

$$
0 + 2(2) + 3(1) = 0 + 4 + 3 = 7.
$$

- **For the entire line $(x, y, z) = (1 + t, t, 2 - t)$:** substituting into the left-hand side for an arbitrary $t \in \mathbb{R}$ gives

$$
(1 + t) + 2(t) + 3(2 - t) = 1 + t + 2t + 6 - 3t = 7.
$$

Since the identity holds for all $t \in \mathbb{R}$, both $P$ and the entire line lie in the plane $x + 2y + 3z = 7$.