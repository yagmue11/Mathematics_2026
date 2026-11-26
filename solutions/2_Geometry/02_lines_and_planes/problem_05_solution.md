### Exercise 5. Relative Position of Two Lines

Analyze the position of

$$
L_1:(x,y,z)=(1,1,0)+t(1,2,1),
$$

$$
L_2:(x,y,z)=(2,0,1)+s(0,1,-1).
$$

If they intersect, give the intersection point. If not, determine whether they are parallel or skew. Justify the classification.

### Solution

**1. Check for parallelism**

The direction vectors of $L_1$ and $L_2$ are

$$
v_1 = (1, 2, 1), \qquad v_2 = (0, 1, -1).
$$

Because the first component of $v_2$ is $0$ while the first component of $v_1$ is $1$, there is no scalar $\lambda \in \mathbb{R}$ such that $v_1 = \lambda v_2$. Thus $v_1$ and $v_2$ are not collinear, so $L_1$ and $L_2$ are neither parallel nor coincident.

**2. Check for intersection**

Equating the parametric coordinates of $L_1$ and $L_2$ gives the system

$$
\begin{cases}
1 + t = 2, \\
1 + 2t = s, \\
t = 1 - s.
\end{cases}
$$

- From the first equation: $t = 2 - 1 = 1$.
- Substituting $t = 1$ into the second equation: $s = 1 + 2(1) = 3$.
- Substituting $t = 1$ and $s = 3$ into the third equation:

$$
1 = 1 - 3 = -2,
$$

which is a contradiction.

**3. Classification**

The system has no solution, so $L_1$ and $L_2$ do not intersect. Since the two lines are neither parallel nor intersecting, they are **skew lines**.