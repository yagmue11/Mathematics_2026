### Exercise 2. A Line in Space

Given

$$L:(x,y,z)=(2,-1,3)+t(1,2,-2).$$

State a point on the line and its direction vector, check whether $P=(4,3,-1)$ lies on $L$, and find the point corresponding to $t=-1$.

### Solution

**1. Point and direction vector**

From the parametric representation $L : p + tv$, a base point on the line is

$$p = (2, -1, 3),$$

and a direction vector of the line is

$$v = (1, 2, -2).$$

**2. Checking whether $P=(4,3,-1)$ lies on $L$**

The point $P$ lies on $L$ if and only if there exists a single scalar $t \in \mathbb{R}$ satisfying

$$(4, 3, -1) = (2, -1, 3) + t(1, 2, -2).$$

Equating coordinates gives the system

$$\begin{cases} 2 + t = 4, \\ -1 + 2t = 3, \\ 3 - 2t = -1. \end{cases}$$

Solving each equation for $t$:

- From the first equation: $t = 4 - 2 = 2$.
- From the second equation: $2t = 4 \implies t = 2$.
- From the third equation: $-2t = -4 \implies t = 2$.

Since all three equations hold for the same parameter value $t = 2$, the point $P=(4,3,-1)$ lies on $L$.

**3. Point corresponding to $t=-1$**

Substituting $t = -1$ into the equation of $L$ gives

$$(x,y,z) = (2, -1, 3) + (-1)(1, 2, -2) = (2 - 1, -1 - 2, 3 + 2) = (1, -3, 5).$$

The point on $L$ corresponding to $t=-1$ is $(1, -3, 5)$.