### Exercise 12. Recognizing a Surface from Cross-Sections

A certain surface has the following properties:
- the cross-section $z=0$ is a point,
- for $z>0$, the cross-sections $z=\mathrm{const}$ are circles with increasing radius,
- vertical cross-sections through the $Oz$ axis are parabolas.

Propose a simple equation for such a surface and justify your choice.

### Solution

**1. Proposed equation**

A simple equation with all three properties is the circular paraboloid

$$
z = x^2 + y^2
$$

*(more generally, $z = a(x^2 + y^2)$ for any constant $a > 0$)*.

**2. Justification of each property**

- **Cross-section $z = 0$ is a point:** Setting $z = 0$ gives $x^2 + y^2 = 0$. Over the real numbers, the only solution is $x = 0$ and $y = 0$, which is the single point $(0, 0, 0)$.
- **Horizontal cross-sections for $z > 0$ are circles of increasing radius:** Setting $z = c > 0$ gives $x^2 + y^2 = c$, which is a circle centered on the $z$-axis at $(0, 0, c)$ with radius $r(c) = \sqrt{c}$. Because $\sqrt{c}$ is a strictly increasing function of $c > 0$, the circles widen monotonically as $z$ increases (and for $z < 0$ there are no points).
- **Vertical cross-sections through the $Oz$ axis are parabolas:** Any vertical plane containing the $z$-axis can be parameterized in cylindrical angle $\theta$ as $x = u\cos\theta$, $y = u\sin\theta$ for $u \in \mathbb{R}$ (for instance, $y = 0$ corresponds to $\theta = 0$ and $x = 0$ corresponds to $\theta = \frac{\pi}{2}$). Substituting into the surface equation gives

$$
z = (u\cos\theta)^2 + (u\sin\theta)^2 = u^2(\cos^2\theta + \sin^2\theta) = u^2,
$$

which is a standard upward-opening parabola in every vertical plane through the $Oz$ axis.