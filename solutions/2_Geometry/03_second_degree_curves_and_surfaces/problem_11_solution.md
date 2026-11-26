### Exercise 11. Two Similar Surfaces

Compare

$$
x^2+y^2-z^2=1
$$

and

$$
x^2+y^2-z^2=-1.
$$

For several values $z=c$, check whether the cross-section exists and what its radius is. Based on this, describe qualitatively the difference between the surfaces and make sketches.

### Solution

**1. Cross-sections $z = c$ for $S_1 : x^2 + y^2 - z^2 = 1$**

Setting $z = c$ gives

$$
x^2 + y^2 = 1 + c^2.
$$

Since $1 + c^2 \ge 1 > 0$ for every $c \in \mathbb{R}$, a circular cross-section of radius $r(c) = \sqrt{1 + c^2}$ exists at every height $z = c$:

- At $c = 0$: circle of minimum radius $r(0) = \sqrt{1} = 1$ (the waist in the $xy$-plane).
- At $c = \pm 1$: circle of radius $r(\pm 1) = \sqrt{2}$.
- At $c = \pm 2$: circle of radius $r(\pm 2) = \sqrt{5}$.

**2. Cross-sections $z = c$ for $S_2 : x^2 + y^2 - z^2 = -1$**

Setting $z = c$ gives

$$
x^2 + y^2 = c^2 - 1.
$$

The cross-section exists only when $c^2 - 1 \ge 0$, i.e., $|c| \ge 1$:

- At $c = 0$: $x^2 + y^2 = -1$, which has **no real points** (empty cross-section).
- At $c = \pm 1$: $x^2 + y^2 = 0$, two single vertex points $(0, 0, 1)$ and $(0, 0, -1)$ (radius $r = 0$).
- At $c = \pm 2$: circle of radius $r(\pm 2) = \sqrt{4 - 1} = \sqrt{3}$.
- At $c = \pm 3$: circle of radius $r(\pm 3) = \sqrt{9 - 1} = \sqrt{8} = 2\sqrt{2}$.

**3. Qualitative comparison and sketches**

- **Surface $S_1$ (hyperboloid of one sheet):** A single connected, hourglass-shaped tube symmetric around the $z$-axis. It is narrowest at the circular waist $x^2 + y^2 = 1$ in the plane $z = 0$ and flares outward smoothly as $|z| \to \infty$.
- **Surface $S_2$ (hyperboloid of two sheets):** Consists of two disconnected bowl-shaped sheets separated by the empty gap $-1 < z < 1$. The upper sheet starts at the vertex $(0,0,1)$ and opens upward ($z \ge 1$), while the lower sheet starts at $(0,0,-1)$ and opens downward ($z \le -1$).