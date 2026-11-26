### Exercise 10. Paraboloids

Compare

$$
z=x^2+y^2
$$

and

$$
z=x^2-y^2.
$$

For each surface, describe the cross-sections $x=0$, $y=0$, and $z=c$, then make a qualitative sketch.

### Solution

**1. Elliptic (circular) paraboloid: $z = x^2 + y^2$**

- **Cross-section $x = 0$ (in the $yz$-plane):** $z = y^2$, an upward-opening parabola with vertex at $(0,0,0)$.
- **Cross-section $y = 0$ (in the $xz$-plane):** $z = x^2$, an upward-opening parabola with vertex at $(0,0,0)$.
- **Horizontal cross-sections $z = c$:**
  - For $c > 0$: $x^2 + y^2 = c$, a circle of radius $\sqrt{c}$ centered at $(0,0,c)$.
  - For $c = 0$: $x^2 + y^2 = 0$, the single vertex point $(0,0,0)$.
  - For $c < 0$: empty (no real points).
- **Qualitative sketch:** A bowl-shaped surface with vertex at the origin, opening upward along the positive $z$-axis with circular horizontal slices.

**2. Hyperbolic paraboloid: $z = x^2 - y^2$**

- **Cross-section $x = 0$ (in the $yz$-plane):** $z = -y^2$, a **downward-opening** parabola with vertex at $(0,0,0)$.
- **Cross-section $y = 0$ (in the $xz$-plane):** $z = x^2$, an **upward-opening** parabola with vertex at $(0,0,0)$.
- **Horizontal cross-sections $z = c$:**
  - For $c > 0$: $x^2 - y^2 = c$, a hyperbola opening along the $x$-direction with vertices at $(\pm\sqrt{c}, 0, c)$.
  - For $c = 0$: $x^2 - y^2 = 0 \implies y = \pm x$, two intersecting straight lines in the $xy$-plane.
  - For $c < 0$: $y^2 - x^2 = -c$, a hyperbola opening along the $y$-direction with vertices at $(0, \pm\sqrt{-c}, c)$.
- **Qualitative sketch:** A saddle-shaped surface centered at the saddle point $(0,0,0)$, curving upward along the $x$-axis and downward along the $y$-axis.

**3. Summary comparison**

| Cross-section | $z = x^2 + y^2$ | $z = x^2 - y^2$ |
| :--- | :--- | :--- |
| $x = 0$ | Parabola $z = y^2$ (opens up) | Parabola $z = -y^2$ (opens down) |
| $y = 0$ | Parabola $z = x^2$ (opens up) | Parabola $z = x^2$ (opens up) |
| $z = c > 0$ | Circle $x^2 + y^2 = c$ | Hyperbola $x^2 - y^2 = c$ ($x$-branches) |
| $z = 0$ | Single point $(0,0,0)$ | Two lines $y = \pm x$ |
| $z = c < 0$ | Empty | Hyperbola $y^2 - x^2 = -c$ ($y$-branches) |