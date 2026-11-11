### Exercise 11. A Parameter in a System of Three Equations
Analyze the number of solutions depending on $t$:

$$
\begin{cases}
x+y+z=1, \\
x+ty+z=2, \\
x+y+tz=3.
\end{cases}
$$

Use elimination and separately analyze the parameter values for which a standard calculation step ceases to be valid.

### Exercise 11. Solution

Subtracting the first equation from the second and third gives the equivalent system

$$
\begin{cases}
x+y+z=1, \\
(t-1)y=1, \\
(t-1)z=2. \\
\end{cases}
$$

**Case $t\neq 1$.** Dividing by $t-1$ determines $y$ and $z$ uniquely. Substituting into the first equation then determines $x$.

$$
\begin{aligned}
y &= \frac{1}{t-1}, \\
z &= \frac{2}{t-1}, \\
x &= 1-y-z = \frac{t-4}{t-1}.
\end{aligned}
$$

**Case $t=1$.** Division by $t-1$ is undefined. The second equation of the reduced system becomes $0=1$, so the system is inconsistent.

Thus the system has **one solution** for every $t\neq 1$ and **no solutions** for $t=1$.