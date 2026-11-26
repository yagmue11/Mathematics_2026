### Exercise 14. Cone and Cylinder

Compare

$$
x^2+y^2=z^2
$$

and

$$
x^2+y^2=4.
$$

For each surface, describe the cross-sections $z=c$, $x=0$, and $y=0$, make a sketch, and explain why the radius of the cross-section depends on $z$ in the first case but is constant in the second.

### Solution

**1. Circular cone: $x^2 + y^2 = z^2$**

- **Cross-section $z = c$:** $x^2 + y^2 = c^2$, a circle centered at $(0,0,c)$ of radius $r = |c|$ for $c \neq 0$, and the single vertex point $(0,0,0)$ when $c = 0$.
- **Cross-section $x = 0$ (in the $yz$-plane):** $y^2 = z^2 \implies z = \pm y$, two intersecting straight lines passing through the origin at $45^\circ$.
- **Cross-section $y = 0$ (in the $xz$-plane):** $x^2 = z^2 \implies z = \pm x$, two intersecting straight lines passing through the origin at $45^\circ$.
- **Sketch description:** A double-napped right circular cone with apex at $(0,0,0)$, expanding linearly upward ($z > 0$) and downward ($z < 0$) around the $z$-axis.

**2. Circular cylinder: $x^2 + y^2 = 4$**

- **Cross-section $z = c$:** $x^2 + y^2 = 4$, a circle centered at $(0,0,c)$ of constant radius $r = 2$ for every $c \in \mathbb{R}$.
- **Cross-section $x = 0$ (in the $yz$-plane):** $y^2 = 4 \implies y = \pm 2$, two parallel vertical lines in the $yz$-plane.
- **Cross-section $y = 0$ (in the $xz$-plane):** $x^2 = 4 \implies x = \pm 2$, two parallel vertical lines in the $xz$-plane.
- **Sketch description:** An infinite vertical tube of radius $2$ centered along the $z$-axis.

**3. Why the radius depends on $z$ in the first case but not the second**

- In $x^2 + y^2 = z^2$, the variable $z$ appears explicitly on the right-hand side, coupling the horizontal radial distance $\sqrt{x^2 + y^2}$ directly to height via $\sqrt{x^2 + y^2} = |z|$. As $|z|$ grows, the cross-section scales proportionally.
- In $x^2 + y^2 = 4$, the variable $z$ does not appear in the equation at all (its coefficient is $0$). Consequently, $z$ is unconstrained, and any point $(x, y, 0)$ on the base circle $x^2 + y^2 = 4$ generates an entire vertical line $(x, y, z)$ parallel to the $z$-axis, keeping the cross-sectional radius fixed at $r = 2$ at every height.