### Exercise 15. Recognition and Sketch Without a Given Name

Consider the two equations:

$$
4x^2+9y^2-8x+36y+4=0,
$$

$$
4x^2+y^2=z^2.
$$

For the first equation, reduce it to canonical form, recognize the curve, give its most important features, and make a sketch.

For the second equation, do not begin by using a ready-made name for the surface. First describe the cross-sections $z=c$ and the cross-sections by the planes $x=0$ and $y=0$, paying attention to the different scales along the axes. Only then identify the surface and make a sketch.

### Solution

**Part 1. First equation: $4x^2 + 9y^2 - 8x + 36y + 4 = 0$**

1. **Canonical form:** Group variables and complete the square:

$$
4(x^2 - 2x) + 9(y^2 + 4y) = -4,
$$

$$
4(x^2 - 2x + 1 - 1) + 9(y^2 + 4y + 4 - 4) = -4,
$$

$$
4(x - 1)^2 - 4 + 9(y + 2)^2 - 36 = -4,
$$

$$
4(x - 1)^2 + 9(y + 2)^2 = 36.
$$

Dividing by $36$ yields

$$
\frac{(x - 1)^2}{9} + \frac{(y + 2)^2}{4} = 1.
$$

2. **Curve type and features:**
   - **Curve:** Shifted **ellipse**.
   - **Center:** $(1, -2)$.
   - **Semiaxes:** Horizontal semiaxis $a = 3$, vertical semiaxis $b = 2$.
   - **Vertices:** $(1 \pm 3, -2)$, i.e., $(-2, -2)$ and $(4, -2)$.
   - **Co-vertices:** $(1, -2 \pm 2)$, i.e., $(1, -4)$ and $(1, 0)$ (tangent to the $x$-axis at $(1,0)$).
   - **Foci:** $c = \sqrt{9 - 4} = \sqrt{5}$, located at $(1 \pm \sqrt{5}, -2)$.
3. **Sketch description:** A horizontal oval centered at $(1, -2)$, spanning horizontally from $x = -2$ to $x = 4$ and vertically from $y = -4$ to $y = 0$, touching the $x$-axis at $(1,0)$.

---

**Part 2. Second equation: $4x^2 + y^2 = z^2$**

1. **Cross-sections by planes $z = c$:**
   - For $c = 0$: $4x^2 + y^2 = 0$, which gives only the single point $(0, 0, 0)$.
   - For $c \neq 0$: dividing $4x^2 + y^2 = c^2$ by $c^2$ yields

$$
\frac{x^2}{\left(\frac{|c|}{2}\right)^2} + \frac{y^2}{|c|^2} = 1.
$$

Each horizontal slice at height $z = c \neq 0$ is an **ellipse** centered at $(0, 0, c)$ whose semiaxes grow linearly with $|c|$:

$$
a(c) = \frac{|c|}{2} \quad \text{(along } x\text{)}, \qquad b(c) = |c| \quad \text{(along } y\text{)}.
$$

Thus every horizontal slice is twice as wide along the $y$-direction as along the $x$-direction.

2. **Cross-sections by the coordinate planes $x = 0$ and $y = 0$:**
   - For $x = 0$ (in the $yz$-plane): $y^2 = z^2 \implies z = \pm y$, a pair of lines through the origin with slope $\pm 1$.
   - For $y = 0$ (in the $xz$-plane): $4x^2 = z^2 \implies z = \pm 2x$, a steeper pair of lines through the origin with slope $\pm 2$.

3. **Identification and sketch:**
   - **Surface identification:** Because the surface is formed by straight lines through the vertex $(0,0,0)$ and its horizontal cross-sections are similar ellipses scaling linearly with $|z|$, the surface is an **elliptic double cone** (elliptic cone) with vertex at the origin and axis along the $z$-axis.
   - **Sketch description:** Two opposite cone nappes meeting at $(0,0,0)$, opening upward ($z > 0$) and downward ($z < 0$). Its cross-sections are ellipses elongated by a factor of $2$ along the $y$-axis relative to the $x$-axis, bounded by steeper generating lines ($z = \pm 2x$) in the $xz$-plane than in the $yz$-plane ($z = \pm y$).