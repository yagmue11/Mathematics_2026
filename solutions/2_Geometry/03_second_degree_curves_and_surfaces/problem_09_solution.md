### Exercise 9. Ellipsoid and Its Cross-Sections

Consider

$$
\frac{x^2}{9}+\frac{y^2}{4}+\frac{z^2}{16}=1.
$$

Give the semiaxis lengths, describe the cross-section $z=0$, and explain how the cross-sections $z=c$ change for $|c|<4$.

### Solution

**1. Semiaxis lengths**

Rewriting the denominators as squares gives

$$
\frac{x^2}{3^2} + \frac{y^2}{2^2} + \frac{z^2}{4^2} = 1.
$$

The semiaxis lengths are:

- along the $x$-axis: $a = 3$,
- along the $y$-axis: $b = 2$,
- along the $z$-axis: $c_z = 4$.

**2. Cross-section at $z = 0$**

Setting $z = 0$ in the equation yields

$$
\frac{x^2}{9} + \frac{y^2}{4} = 1, \qquad z = 0.
$$

This is an ellipse in the $xy$-plane centered at $(0,0,0)$ with horizontal semiaxis $3$ and vertical semiaxis $2$.

**3. Evolution of cross-sections $z = c$ for $|c| < 4$**

For a horizontal plane $z = c$ with $|c| < 4$, substituting $z = c$ gives

$$
\frac{x^2}{9} + \frac{y^2}{4} = 1 - \frac{c^2}{16}.
$$

Since $1 - \frac{c^2}{16} > 0$, dividing through by $1 - \frac{c^2}{16}$ yields

$$
\frac{x^2}{9\left(1 - \frac{c^2}{16}\right)} + \frac{y^2}{4\left(1 - \frac{c^2}{16}\right)} = 1.
$$

- Every horizontal cross-section for $|c| < 4$ is an **ellipse** centered at $(0, 0, c)$ with semiaxes

$$
a(c) = 3\sqrt{1 - \frac{c^2}{16}}, \qquad b(c) = 2\sqrt{1 - \frac{c^2}{16}},
$$

maintaining the constant aspect ratio $\frac{a(c)}{b(c)} = \frac{3}{2}$.
- The ellipse is largest at the equator $c = 0$ ($a = 3, b = 2$) and shrinks smoothly as $|c|$ increases toward $4$.
- At the poles $c = \pm 4$, the cross-section degenerates into the single points $(0, 0, 4)$ and $(0, 0, -4)$, and for $|c| > 4$ the cross-section is empty.