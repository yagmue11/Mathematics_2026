### Exercise 12. Intersection Line of Two Planes

Find a parametric equation of the line that is the intersection of

$$
x+y+z=3,\qquad x-y+z=1.
$$

Find its direction vector in two ways: from the system of equations and from the cross product of the normal vectors. Compare the results.

### Solution

**1. Parametric equation from the linear system**

Solve the system of two linear equations:

$$
\begin{cases}
x + y + z = 3, \\
x - y + z = 1.
\end{cases}
$$

Subtracting the second equation from the first eliminates $x$ and $z$:

$$
(x + y + z) - (x - y + z) = 3 - 1 \implies 2y = 2 \implies y = 1.
$$

Substituting $y = 1$ into the first equation gives

$$
x + 1 + z = 3 \implies x = 2 - z.
$$

Choosing $z = t \in \mathbb{R}$ as the free parameter yields the parametric equations of the intersection line:

$$
\begin{cases}
x = 2 - t, \\
y = 1, \\
z = t,
\end{cases}
\qquad t \in \mathbb{R},
$$

or in vector form,

$$
L : (x, y, z) = (2, 1, 0) + t(-1, 0, 1).
$$

From this representation, a direction vector is

$$
v_{\mathrm{sys}} = (-1, 0, 1).
$$

**2. Direction vector from the cross product of the normals**

The normal vectors of the two planes are

$$
n_1 = (1, 1, 1), \qquad n_2 = (1, -1, 1).
$$

Since the intersection line lies in both planes, its direction must be orthogonal to both $n_1$ and $n_2$:

$$
\begin{aligned}
v_{\mathrm{cross}} &= n_1 \times n_2 \\
                   &= (1, 1, 1) \times (1, -1, 1) \\
                   &= (1(1) - 1(-1),\; 1(1) - 1(1),\; 1(-1) - 1(1)) \\
                   &= (2, 0, -2).
\end{aligned}
$$

**3. Comparison**

Comparing the two direction vectors shows that

$$
v_{\mathrm{cross}} = (2, 0, -2) = -2(-1, 0, 1) = -2v_{\mathrm{sys}}.
$$

The two vectors are nonzero scalar multiples of each other, so they define the exact same direction in $\mathbb{R}^3$ (differing only in length and orientation).