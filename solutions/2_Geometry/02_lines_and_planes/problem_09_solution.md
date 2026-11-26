### Exercise 9. Distances

Compute:

1. the distance from $P=(2,3)$ to the line $3x+4y-10=0$,
2. the distance from $Q=(2,-1,3)$ to the plane $2x-2y+z-4=0$.

Compare the two formulas and explain their common connection with the normal direction.

### Solution

**1. Distance from $P=(2,3)$ to the line $3x+4y-10=0$**

Using the point-to-line distance formula in $\mathbb{R}^2$,

$$
d(P, L) = \frac{|ax_0 + by_0 + c|}{\sqrt{a^2 + b^2}},
$$

with $(a,b,c) = (3,4,-10)$ and $(x_0,y_0) = (2,3)$:

$$
d(P, L) = \frac{|3(2) + 4(3) - 10|}{\sqrt{3^2 + 4^2}} = \frac{|6 + 12 - 10|}{\sqrt{9 + 16}} = \frac{8}{5}.
$$

**2. Distance from $Q=(2,-1,3)$ to the plane $2x-2y+z-4=0$**

Using the point-to-plane distance formula in $\mathbb{R}^3$,

$$
d(Q, \Pi) = \frac{|ax_0 + by_0 + cz_0 + d|}{\sqrt{a^2 + b^2 + c^2}},
$$

with $(a,b,c,d) = (2,-2,1,-4)$ and $(x_0,y_0,z_0) = (2,-1,3)$:

$$
d(Q, \Pi) = \frac{|2(2) - 2(-1) + 1(3) - 4|}{\sqrt{2^2 + (-2)^2 + 1^2}} = \frac{|4 + 2 + 3 - 4|}{\sqrt{4 + 4 + 1}} = \frac{5}{3}.
$$

**3. Comparison and geometric connection**

Both formulas are special cases of the same vector projection identity in $\mathbb{R}^m$ ($m=2$ for a line in the plane, $m=3$ for a plane in space). A hyperplane defined by $n \cdot x + d = 0$ has normal vector $n$, and any point $x_1$ on it satisfies $d = -n \cdot x_1$. For an arbitrary point $x_0$, the shortest segment to the hyperplane runs parallel to $n$, so its length is the absolute scalar projection of $x_0 - x_1$ onto the unit normal $\frac{n}{\|n\|}$:

$$
\mathrm{dist} = \left| \frac{n}{\|n\|} \cdot (x_0 - x_1) \right| = \frac{|n \cdot x_0 - n \cdot x_1|}{\|n\|} = \frac{|n \cdot x_0 + d|}{\|n\|}.
$$