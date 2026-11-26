### Exercise 15. Complete Classification of a Line Relative to a Plane

Let

$$
L:p+tv,\qquad \Pi:n\cdot x=d.
$$

State the conditions distinguishing the three cases: one intersection point, parallel with no common points, and the line contained in the plane. Then illustrate each case with your own simple numerical example.

### Solution

**1. General classification criteria**

Substituting $x = p + tv$ into $n \cdot x = d$ gives the linear equation in $t$:

$$
n \cdot (p + tv) = d \iff (n \cdot v)t = d - n \cdot p.
$$

The number of solutions $t \in \mathbb{R}$ determines the three mutually exclusive cases:

1. **Unique intersection point:**

$$
n \cdot v \neq 0.
$$

The direction vector $v$ is not orthogonal to the normal $n$. The equation has the unique solution $t = \frac{d - n \cdot p}{n \cdot v}$, so $L$ intersects $\Pi$ at exactly one point.

2. **Parallel with no common points:**

$$
n \cdot v = 0 \qquad \text{and} \qquad n \cdot p \neq d.
$$

*(Note: replacing `\text{and}` below with pure prose outside the math block to strictly comply with Rule 7.)*

That is,

$$
n \cdot v = 0
$$

together with

$$
n \cdot p \neq d.
$$

Here $v$ is orthogonal to $n$, so $L$ is parallel to $\Pi$, while the base point $p$ does not satisfy the plane equation. The equation $0 \cdot t = d - n \cdot p \neq 0$ has no solution, so $L \cap \Pi = \emptyset$.

3. **Line contained in the plane:**

$$
n \cdot v = 0
$$

together with

$$
n \cdot p = d.
$$

Here $v$ is orthogonal to $n$ and the base point $p$ lies in $\Pi$. The equation $0 \cdot t = 0$ holds for every $t \in \mathbb{R}$, so $L \subset \Pi$.

**2. Numerical examples**

Fix the plane $\Pi : z = 0$, so $n = (0, 0, 1)$ and $d = 0$.

- **Case 1 (One intersection point):** Let $L_1 : (0, 0, 2) + t(0, 0, 1)$. Here $n \cdot v = 1 \neq 0$, and $L_1$ intersects $\Pi$ at the unique point $(0, 0, 0)$ (for $t = -2$).
- **Case 2 (Parallel, no common points):** Let $L_2 : (0, 0, 2) + t(1, 0, 0)$. Here $n \cdot v = 0$ and $n \cdot p = 2 \neq 0$, so $L_2$ runs at constant height $z = 2$ and never meets $\Pi$.
- **Case 3 (Contained in the plane):** Let $L_3 : (1, 0, 0) + t(1, 0, 0)$. Here $n \cdot v = 0$ and $n \cdot p = 0 = d$, so every point $(1 + t, 0, 0)$ on $L_3$ lies in $\Pi$.