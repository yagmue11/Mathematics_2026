### Exercise 1. Line Through Two Points

Find the equation of the line through $A=(1,2)$ and $B=(4,-1)$ in parametric and general form. Identify a direction vector and an example of a normal vector. Check that both points satisfy the equation you obtain.

### Solution

**1. Direction vector and parametric form**

A direction vector $v$ of the line is given by the displacement vector from $A$ to $B$:

$$v = \overrightarrow{AB} = B - A = (4 - 1, -1 - 2) = (3, -3).$$

Using $A=(1,2)$ as the base point and $v=(3,-3)$ as the direction vector, the parametric equation of the line is

$$(x,y) = (1,2) + t(3,-3), \qquad t \in \mathbb{R},$$

or in component form:

$$\begin{cases} x = 1 + 3t, \\ y = 2 - 3t, \end{cases} \qquad t \in \mathbb{R}.$$

**2. Normal vector and general form**

A normal vector $n = (n_1, n_2)$ in $\mathbb{R}^2$ is orthogonal to $v = (3, -3)$, so $n \cdot v = 0$. Scaling $v$ by $\frac{1}{3}$ gives a simpler collinear direction vector $v_0 = (1, -1)$, from which an example of a normal vector is

$$n = (1, 1).$$

Using the point-normal condition $n \cdot ((x,y) - A) = 0$:

$$1(x - 1) + 1(y - 2) = 0,$$

which simplifies to the general form of the line:

$$x + y - 3 = 0.$$

**3. Verification**

- Substituting $A=(1,2)$ into the general form yields

$$1 + 2 - 3 = 0,$$

and in parametric form, $t = 0$ gives $(x,y) = (1,2)$.

- Substituting $B=(4,-1)$ into the general form yields

$$4 + (-1) - 3 = 0,$$

and in parametric form, $t = 1$ gives $(x,y) = (1+3, 2-3) = (4,-1)$.

Both points satisfy both forms of the equation.