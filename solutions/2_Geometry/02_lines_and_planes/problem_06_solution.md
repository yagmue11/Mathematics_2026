### Exercise 6. Angle Between Planes

Given

$$
\Pi_1:x+y+z=1,\qquad \Pi_2:x-y=2.
$$

First use the normal vectors to decide whether the planes are parallel. If not, compute the angle between them and explain why the normal vectors alone are enough for this calculation.

### Solution

**1. Normal vectors and parallelism check**

Reading the coefficients of $(x,y,z)$ from each plane equation gives the normal vectors

$$
n_1 = (1, 1, 1), \qquad n_2 = (1, -1, 0).
$$

Since the third component of $n_2$ is $0$ while that of $n_1$ is $1$, $n_1$ is not a scalar multiple of $n_2$. Therefore, the planes $\Pi_1$ and $\Pi_2$ are not parallel and must intersect along a line.

**2. Angle between the planes**

The acute (or right) dihedral angle $\theta \in [0, \frac{\pi}{2}]$ between $\Pi_1$ and $\Pi_2$ satisfies

$$
\cos\theta = \frac{|n_1 \cdot n_2|}{\|n_1\|\,\|n_2\|}.
$$

Computing the dot product and the norms:

$$
n_1 \cdot n_2 = 1(1) + 1(-1) + 1(0) = 0,
$$

$$
\|n_1\| = \sqrt{1^2 + 1^2 + 1^2} = \sqrt{3}, \qquad \|n_2\| = \sqrt{1^2 + (-1)^2 + 0^2} = \sqrt{2}.
$$

Substituting these values into the cosine formula gives

$$
\cos\theta = \frac{|0|}{\sqrt{3}\sqrt{2}} = 0 \implies \theta = \frac{\pi}{2} \quad (90^\circ).
$$

The two planes are perpendicular.

**3. Why normal vectors alone suffice**

Rotating a plane by an angle $\theta$ rotates its perpendicular direction by the exact same angle $\theta$. In the cross-sectional plane perpendicular to the line of intersection of $\Pi_1$ and $\Pi_2$, the two normal vectors lie in that cross-section and are rotated by $90^\circ$ relative to the plane traces, preserving the angle between them.