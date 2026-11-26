### Exercise 5. Hyperbola and Asymptotes

For

$$
\frac{x^2}{16}-\frac{y^2}{9}=1,
$$

find the intercepts with the $x$-axis, the asymptotes, and make a sketch. Explain why the asymptotes describe the behavior of the curve far from the center.

### Solution

**1. Intercepts with the $x$-axis**

Setting $y = 0$ in the equation gives

$$
\frac{x^2}{16} = 1 \implies x^2 = 16 \implies x = \pm 4.
$$

The $x$-intercepts (vertices) are $(-4, 0)$ and $(4, 0)$. (Setting $x = 0$ gives $-\frac{y^2}{9} = 1$, which has no real solutions, so there are no $y$-intercepts.)

**2. Asymptotes**

Replacing the right-hand side $1$ by $0$ gives the equation of the asymptotes:

$$
\frac{x^2}{16} - \frac{y^2}{9} = 0 \implies \frac{y^2}{9} = \frac{x^2}{16} \implies y = \pm\frac{3}{4}x.
$$

The two asymptotes are the lines $y = \frac{3}{4}x$ and $y = -\frac{3}{4}x$.

**3. Sketch and asymptotic behavior**

- **Sketch description:** Draw the central rectangle $[-4, 4] \times [-3, 3]$ and extend its two diagonals $y = \pm\frac{3}{4}x$. Sketch the two branches of the hyperbola starting vertically at the vertices $(-4,0)$ and $(4,0)$, opening left and right respectively, and approaching the diagonal asymptotes without crossing them.
- **Why asymptotes govern behavior far from the center:** Solving the hyperbola equation for $y$ gives

$$
y = \pm\frac{3}{4}\sqrt{x^2 - 16} = \pm\frac{3}{4}|x|\sqrt{1 - \frac{16}{x^2}}.
$$

When $|x|$ is very large ($|x| \gg 4$), the term $\frac{16}{x^2}$ approaches $0$, so $\sqrt{1 - \frac{16}{x^2}} \approx 1$ and $y \approx \pm\frac{3}{4}x$. Geometrically, the constant $1$ on the right-hand side becomes negligible compared to $\frac{x^2}{16}$ and $\frac{y^2}{9}$ far from the origin.